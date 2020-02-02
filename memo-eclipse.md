# Mémo Eclipse

par *flashjaysan*

## Importer un projet Git dans Eclipse

- Dans Eclipse, cliquez sur le menu `File -> Import...`.
- Dans la boîte de dialogue `Import`, sélectionnez `Git -> Projects from Git` puis cliquez sur `Next`.
- Dans la boîte de dialogue `Import Projects from Git`, Sélectionnez `Clone URI` puis cliquez sur `Next`.
- Collez l'adresse du projet Git dans le champ `URI` puis cliquez sur `Next`.
- Cochez la branche à cloner (`master`) puis cliquez sur `Next`.
- Dans le champ `Directory`, définissez un dossier vide. Vérifiez que le champ `Remote name` fasse bien référence au bon projet puis cliquez sur `Next`.
- Sélectionnez l'option `Import as general project` puis cliquez sur `Next`.
- Dans le champ `Project name`, définissez le nom du projet puis cliquez sur `Finish`.

## Définir la nature d'un projet Maven

- Dans le panneau `Package Explorer`, faites un clic droit sur la racine du projet puis sélectionnez `Properties`.
- Dans la boîte de dialogue `Properties for *nom_du_projet*`, sélectionnez l'option `Project Natures`.
- Cliquez sur le bouton `Add`.
- Si la boîte de dialogue `Confirm nature update` apparaît, cliquez sur le bouton `OK`.
- Dans la boîte de dialogue `Select Nature`, sélectionnez l'option `Maven Nature` puis cliquez sur le bouton `OK`.
- Cliquez sur le bouton `Apply and close`.
- Dans le panneau `Package Explorer`, faites un clic droit sur la racine du projet puis sélectionnez `Maven -> Update Project...`.
- Dans la boîte de dialogue `Update Maven Project`, cochez le projet à mettre à jour puis cliquez sur `OK`.
- Dans le panneau `Package Explorer`, faites un clic droit sur la racine du projet puis sélectionnez `Run As -> Maven Install`.

**Attention !** Pour fonctionner, le projet autour de *JDBC-JAXB* de Martin nécessite d'éditer le fichier `db-products.properties` dans le dossier `src/main/resources`.

- Les propriétés `database` et `user` sont identiques et correspondent à votre identifiant.
- La propriété `password` correspond à votre mot de passe.
- Sauvegardez ce fichier et refaites un `Maven Install`.
