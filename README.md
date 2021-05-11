# Book Store

## Introducere

Aflându-ne într-un context pandemic ce ne îndeamnă la izolare sau la petrecut mult mai mult timp acasă în solitudine, carțile reprezintă un bun refugiu spiritual și mental pentru noi, de aceea, este foarte important ca oamenii să aibă acces ușor la achiziționarea de cărți, fără a trebui să se deplaseze la bibliotecă sau la alte magazine destinate. Astfel, aplicația realizată de mine reprezintă un online-shop pentru cărți, prin care utilizatorul poate vizualiza și rating-urile cărților prezentate.

## Descriere problemă
Pandemia a avut ca efect imediat închiderea încăperilor ce pot reprezenta pericole din punct de vedere al aglomerării sociale, printre acestea incluzându-se și bibliotecile sau magazinele de cărți. De asemenea, odată cu sporirea lucrului în regim de telemuncă, majoritatea petrec mult mai mult timp acasă, astfel, preferând cumpărăturile de tip online. 
Aplicația realizată de mine vine în ajutorul acestora și nu numai, prin facilitarea accesului la o gama largă și variată de cărți, precum și achiziționarea acestora.

Pagina principala a aplicației:

Am ales o pagină principală simplistă, cu o listă de cărți, două butoane pentru editarea și ștergerea cărților și un buton pentru adăugarea unei noi cărți.
 

## Descriere API-uri
Pentru partea de back-end am folosit fake Json(JsonServer), iar cu ajutorul acestui server am realizat următoarele API-uri.
### •	API-ul de POST, ce permite publicarea cărților din Json

https://imgur.com/a/4r1mAqJ
 
### •	API-ul de put – ce are rolul de a updata cărțile după ce acestea au fost editate de către utilizator

https://imgur.com/a/8S36sNs

### •	API de delete – ce are rolul de șterge cărțile din tabelul paginii și a updata pagina

https://imgur.com/a/e6LBRFn

### •	API pentru adăugarea unei noi cărți după utilizarea butonului de Add Book

https://imgur.com/a/LO2hvVz
             

## Fluxul de date
```javascript
axios.post("http://localhost:3000/books", this.state.newBookData)
    .then((response) => {
      let {books} = this.state; 
      book.push(response.data);
```

Metodele HTTP folosite sunt cele de get și post.


## Capturi de ecran din aplicatie

https://imgur.com/a/odwqbMS

https://imgur.com/a/CTdcmvf


 
