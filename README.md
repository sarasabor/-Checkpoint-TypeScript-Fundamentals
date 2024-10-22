# -Checkpoint-TypeScript-Fundamentals



Voici comment vous pouvez résoudre cet exercice en TypeScript :

Définir l'interface Véhicule.
Implémenter la classe Voiture.
Créer une instance de Voiture et appeler la méthode start.
Voici le code :

typescript
Copier le code
// Définition de l'interface Véhicule
interface Véhicule {
    make: string;
    model: string;
    year: number;
    start(): void;
}

// Implémentation de la classe Voiture
class Voiture implements Véhicule {
    make: string;
    model: string;
    year: number;

    constructor(make: string, model: string, year: number) {
        this.make = make;
        this.model = model;
        this.year = year;
    }

    start(): void {
        console.log("Car engine started");
    }
}

// Création d'une instance de la classe Voiture
const maVoiture = new Voiture("Toyota", "Corolla", 2020);

// Appel de la méthode start
maVoiture.start();
Étapes suivantes :
Compiler le code TypeScript : Utilisez la commande suivante dans votre terminal :

bash
Copier le code
tsc nomDuFichier.ts
Exécuter le code JavaScript : Utilisez Node.js pour exécuter le fichier compilé :

bash
Copier le code
node nomDuFichier.js
Cela devrait afficher "Car engine started" dans la console
