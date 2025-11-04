# sweet-cravings
Digital bakery management app — catalog, cart &amp; orders for users; admin dashboard for products, users, orders &amp; deliveries (ASP.NET MVC).

# Sweet Cravings 🍰 — Bakery Management (ASP.NET MVC)

Application web pour une boulangerie/pâtisserie :
- **Côté client** : catalogue, panier, commande, historique, avis.
- **Côté admin** : gestion produits/utilisateurs/livreurs, affectation & suivi des commandes, tableau de bord.
- **Livreur** : liste des commandes assignées, mise à jour des statuts.

## ✨ Fonctionnalités
- Authentification & rôles (User, Admin, Deliverer)
- Catalogue produits (catégories, prix, promo, allergènes)
- Panier + passage de commande
- Gestion commandes (affectation livreur, statuts: pending/validated/delivered)
- Avis/commentaires produits
- Tableau de bord (ventes, livraisons)
- (Optionnel) Caisse / suivi transactions

## 🧱 Modèles principaux (extrait)
- **User**(Id, Name, Email, Role)
- **Product**(Id, Name, Price, Category, ImageUrl, IsActive, Promo)
- **CartItem**(Id, UserId, ProductId, Qty)
- **Order**(Id, UserId, CreatedAt, Total, Status)
- **OrderItem**(OrderId, ProductId, Qty, UnitPrice)
- **Delivery**(Id, OrderId, Address, City, Status, AssignedToDelivererId)
- **Comment**(Id, UserId, ProductId, Text, Rating, CreatedAt)

## 🧰 Stack
- **Back** : ASP.NET MVC (C#)
- **Front** : HTML, CSS, Bootstrap, JavaScript
- **DB** : SQL Server
- **Outils** : UML (StarUML), Figma, Git

## 🚀 Lancer en local
1) Cloner  
```bash
git clone git@github.com:ElJalili/sweet-cravings.git
cd sweet-cravings

