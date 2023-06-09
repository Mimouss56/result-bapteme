<!-- Debut de la correction : 12:02 -->

La relation USER <-> PRODUCT n'est pas bonne
pour rappel, le 1er chiffre correspond au minimum de produit que peut avoir un user, le 2eme chiffre correspond au max
dans ce cas :
- Tu marques que le USER LIKE min(1), max(1) PRODUCT or il peut LIKER 0 ou plusieurs produits
- Dans l'autre sens PRODUCT LIKE USER, on doit comprendre que le produit peut être LIKE par 0 ou plusieurs USER

Il te faut dans ce cas avoir un USER 0,N PRODUCT et un PRODUCT 0,N USER
C'est ce qu'on appelle une relation ManyToMany
Attention tout de fois, une fois que tu as compris que tu as une relation ManyToMany, tu auras besoin d'une table de jointure
Cette table de jointure te permettra de faire le lien entre USER et PRODUCT
Cette table de jointure aura besoin d'avoir 2 clés étrangères, une pour USER et une pour PRODUCT

<!-- Fin de la correction : 12:12 -->
