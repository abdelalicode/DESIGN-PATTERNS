# Singleton Design Pattern

Le design pattern Singleton est un modèle de conception permettant de restreindre l'instanciation d'une classe à un seul objet. Cela signifie qu'une classe Singleton ne peut avoir qu'une seule instance dans toute l'application.

## Utilisation

Le pattern Singleton est souvent utilisé lorsque vous avez besoin d'une seule instance partagée à travers toute votre application, comme par exemple :

- Configuration globale
- Gestionnaire de connexion à une base de données
- Pool d'objets réutilisables

## Implémentation

Voici un exemple d'implémentation d'une classe Singleton en Java :

```java
public class Singleton {
    private static Singleton instance;

        // Constructeur privé pour empêcher l'instanciation directe depuis l'extérieur
        private Singleton() {
                }

        // Méthode statique pour obtenir l'instance unique
        public static Singleton getInstance() {
            if (instance == null) {
                instance = new Singleton();
                }
                return instance;
                                                                }

             // Autres méthodes de la classe Singleton
}

```