# Progetto di Informatica Grafica

Questo progetto consiste nella modellazione e renderizzazione di una scena 3D completa realizzata in Blender, raffigurante un iconico paesaggio montano giapponese con una Toyota Trueno AE86 che percorre i tornanti.

## Descrizione del Progetto
Il lavoro si focalizza sulla creazione di un ambiente realistico ispirato ai passi montani giapponesi (*touge*), caratterizzato da una strada a tornanti con guida a sinistra, strisce gialle centrali e bianche laterali.

---

## Modellazione del Paesaggio
Il terreno è stato generato attraverso un workflow procedurale e tecnico:
* **Distribuzione Irregolare**: Utilizzo di texture *Voronoi*, *Musgrave* e *Noise* per creare variazioni naturali sulla superficie.
* **Geometry Nodes**: Implementazione dei nodi *UV Sphere* e *Geometry Proximity* per controllare la trasformazione del terreno in base alla distanza da un oggetto guida.
* **Shading Dinamico**: Il sistema utilizza un *Mix Shader* basato sulla coordinata Z (pendenza) per applicare l'erba sulle zone pianeggianti e la roccia sulle pareti scoscese.
* **Vegetazione**: Flora composta da alberi modellati da cubi ed estrusioni. Le foglie sono state realizzate con immagini su piani distribuite tramite un sistema *hair emitter*.

## La Strada
La carreggiata segue fedelmente la topografia del monte:
* **Struttura**: Creata tramite una curva e un piano duplicato con il modificatore *Array*.
* **Adattamento**: Utilizzo del modificatore *Shrinkwrap* per far aderire perfettamente l'asfalto alla superficie della montagna.
* **Materiali**: Shading basato su un materiale che simula l'asfalto dettagliato per aumentare il realismo.

## Il Veicolo: Toyota Trueno AE86
Il pezzo forte è l'auto resa celebre dal manga *Initial D*:
* **Modellazione**: Partendo da un cubo, la carrozzeria è stata estrusa sfruttando il *Mirror Modifier* per garantire simmetria.
* **Dettagli**: Rifinitura accurata di cerchioni, tubo di scarico, specchietti, tergicristalli e fari pop-up.
* **Texture**: Livrea classica bianco-nero con scritte giapponesi sulle fiancate e targhe personalizzate.

## Illuminazione e Rendering
L'atmosfera finale è data da un setup di luci curato:
* **Luce Principale**: Una *Sun Light* che simula la luce solare e genera ombre morbide.
* **Sfondo**: Utilizzo di una texture HDRI per fornire profondità e riflessi realistici.
* **Effetti**: Applicazione dell'*Ambient Occlusion* per migliorare il contrasto nelle aree d'ombra.
* **Luci Funzionali**: *Point Light* configurate come spot per i fari anteriori e luci rosse intense per i freni posteriori.

---

**Autore**: Albuzzi Davide  