Intens Api DevOps

Uputstvo za izradu.


Koraci:

Forkovati repozitorijum

Pokrenuti api lokalno koristeci alat po izboru (dodati env variablu PORT i dodeliti vrednost 8080 ili bilo koji drugi dostupan port)

Napisati Dockerfile 

Upraditi deploy apia na bilo koji cloud provider, moze i docker / kubernetes lokalno

Implemetirati CI CD koristeci GitHub Actions, potrebno je kreirati dve ci cd skripte. Prva skripta treba da se pokrece automatski prilikom kreiranja PR nad master granom i treba da izvrsi testove. 2. skripta treba da se pokrece automatski prilikom pusha na master granu i treba da izvrsava build apia, pakovanje i odlaganje docker slike na repo po zelji i zamenu stare za novu sliku na odabranom cloud provideru ili lokalu. 



NAPOMENA:

Resenje poslednjeg zahteva:

U datoteci .github, u workflows datoteci nalaze se dva fajla. U prvom fajlu "CI-CD" je implementirana prva skripta, a u drugom fajlu "CI-CD-2" je implementirana druga skripta.
