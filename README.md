# Progetto di Informatica Grafica

[cite_start]Questo progetto consiste nella modellazione e renderizzazione di una scena 3D completa realizzata in Blender, raffigurante un iconico paesaggio montano giapponese con una Toyota Trueno AE86 che percorre i tornanti[cite: 1, 114]. Se senti una musica Eurobeat in sottofondo mentre leggi, è perfettamente normale.

## Descrizione del Progetto
[cite_start]Il lavoro si focalizza sulla creazione di un ambiente realistico ispirato ai passi montani giapponesi (*touge*), caratterizzato da una strada a tornanti con guida a sinistra, strisce gialle centrali e bianche laterali[cite: 6].

---

## Modellazione del Paesaggio
Il terreno è stato generato attraverso un workflow procedurale e tecnico:
* [cite_start]**Distribuzione Irregolare**: Utilizzo di texture *Voronoi*, *Musgrave* e *Noise* per creare variazioni naturali sulla superficie[cite: 9].
* [cite_start]**Geometry Nodes**: Implementazione dei nodi *UV Sphere* e *Geometry Proximity* per controllare la trasformazione del terreno in base alla distanza da un oggetto guida[cite: 10, 11, 14, 15].
* [cite_start]**Shading Dinamico**: Il sistema utilizza un *Mix Shader* basato sulla coordinata Z (pendenza) per applicare l'erba sulle zone pianeggianti e la roccia sulle pareti scoscese[cite: 25].
* [cite_start]**Vegetazione**: Flora composta da alberi modellati da cubi ed estrusioni[cite: 42]. [cite_start]Le foglie sono state realizzate con immagini su piani distribuite tramite un sistema *hair emitter*[cite: 43].

## La Strada
La carreggiata segue fedelmente la topografia del monte:
* [cite_start]**Struttura**: Creata tramite una curva e un piano duplicato con il modificatore *Array*[cite: 78, 80].
* [cite_start]**Adattamento**: Utilizzo del modificatore *Shrinkwrap* per far aderire perfettamente l'asfalto alla superficie della montagna[cite: 85].
* [cite_start]**Materiali**: Shading basato su un materiale che simula l'asfalto dettagliato per aumentare il realismo[cite: 93].

## Il Veicolo: Toyota Trueno AE86
[cite_start]Il pezzo forte è l'auto resa celebre dal manga *Initial D*[cite: 114]:
* [cite_start]**Modellazione**: Partendo da un cubo, la carrozzeria è stata estrusa sfruttando il *Mirror Modifier* per garantire simmetria[cite: 118, 119, 120].
* [cite_start]**Dettagli**: Rifinitura accurata di cerchioni, tubo di scarico, specchietti, tergicristalli e fari pop-up[cite: 127, 128].
* [cite_start]**Texture**: Livrea classica bianco-nero con scritte giapponesi sulle fiancate e targhe personalizzate (Gunma 55 13-954)[cite: 131, 132, 134].

## Illuminazione e Rendering
L'atmosfera finale è data da un setup di luci curato:
* [cite_start]**Luce Principale**: Una *Sun Light* che simula la luce solare e genera ombre morbide[cite: 109].
* [cite_start]**Sfondo**: Utilizzo di una texture HDRI per fornire profondità e riflessi realistici[cite: 110].
* [cite_start]**Effetti**: Applicazione dell'*Ambient Occlusion* per migliorare il contrasto nelle aree d'ombra[cite: 111].
* [cite_start]**Luci Funzionali**: *Point Light* configurate come spot per i fari anteriori e luci rosse intense per i freni posteriori[cite: 137, 138].

---

[cite_start]**Autore**: Albuzzi Davide (Mat. 879363) [cite: 3]  