# Changelog

Tous les changements notables de ce projet seront documentés dans ce fichier.

Le format est basé sur [Keep a Changelog](https://keepachangelog.com/fr/1.0.0/),
et ce projet adhère à [Semantic Versioning](https://semver.org/lang/fr/).

## [1.0.0] - 2024-01-XX

### Ajouté
- Système de cache complet avec support de multiples drivers
- Driver Array (cache en mémoire)
- Driver File (cache sur disque)
- Driver Redis (nécessite l'extension Redis)
- Système de tags pour invalidation groupée
- Support TTL (Time To Live) avec expiration automatique
- Validation sécurisée des clés de cache
- Sérialisation sécurisée avec JSON
- Opérations multiples (getMultiple, setMultiple, deleteMultiple)
- Incrémentation et décrémentation de valeurs numériques
- Méthode pull() pour récupérer et supprimer en une opération
- Interface fluide avec façade statique Cache
- CacheManager pour gestion avancée
- TaggedCache pour gestion des tags
- Tests unitaires complets
- Documentation complète avec exemples

### Sécurité
- Validation stricte des clés (protection contre les injections de chemins)
- Sérialisation sécurisée avec validation JSON
- Permissions de fichiers contrôlées pour le driver File
- Écriture atomique pour éviter la corruption des données
- Protection contre les caractères spéciaux dans les clés

