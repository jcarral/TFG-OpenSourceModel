# Test

Introducción a los tests de la apliación. En este apartado se deben especificar cuales son las tecnologías que se utilizan y la metología a seguir.

## Ejemplo

```javascript
describe('getSummary: ', () => {
	it('should return an error, parameters required', () => {
		return expect(new Degree().getSummary()).to.be.rejected;
	});

	it('should return an error, school code required', function() {
		return expect(new Degree('GINFOR30').getSummary()).to.be.rejected;
	});

	it('should return an object with all the attributes', () => {
		const sociologia = new Degree('GESOCI30', '354');
		return sociologia.getSummary()
			.then(res => {
				expect(res).to.be.an('object');
				expect(res).to.have.property('name');
				expect(res).to.have.property('href');
				expect(res).to.have.property('summary');
				expect(res).to.have.property('minimum-degree');
				expect(res).to.have.property('contact');
				expect(res.contact).to.be.an('object');
				expect(res.contact).to.have.property('address');
				expect(res.contact).to.have.property('phone');
				expect(res.contact).to.have.property('email'); //Optional
				expect(res).to.have.property('school');
				expect(res.school).to.be.an('object');
				expect(res.school).to.have.property('name');
				expect(res.school).to.have.property('code');
			});
	});
});
```

Escenarios contemplados:
1. Falla porque no recibe parámetros.
2. Falla porque falta un parámetro.
3. La función devuelve un objeto con todos los valores correctos.
