Explorons le test Khi-deux d’indépendance 

Imaginez que vous vendez des maisons et vous voulez savoir si la tranche d’âge influence le type de logement. La question que vous pouvez vous poser :  Est-ce que la tranche d'âge des acheteurs influence le type de logement qu’ils préfèrent acheter ?
Le test de Khi-deux peut vous permettre de faire cela. 

Notre hypothèse business : La tranche d'âge des acheteurs influence le type de logement

Hypothèses statistiques :
•	H0 : L’âge et le type de logement sont indépendants → pas de lien réel.
•	H1 : Il y a une dépendance → l’âge influence le type de logement préféré.
Interprétation :
•	Si p-value < 0.05 → le type de logement dépend significativement de l’âge → stratégie marketing à adapter par tranche d’âge.
•	Si p-value ≥ 0.05 → pas de lien détecté → préférences plus homogènes que prévu.

Âge / Type de logement	Appartement	Maison	Loft	Total	Lignes
< 35 ans	20	10	10	40	1
≥ 35 ans	10	25	5	40	2
Total	30	35	15	80	
Colonnes	1	2	3		

Calculons manuellement :  E11 : Calcul ligne 1, colonne 1 soit (Appart, < 35)
-	E11 = (Total première ligne × Total première colonne) / Total général | E11= (40 × 30)/80 = 15   
-	Nous avons pour la cellule Appart, < 35 alors : (O11-E11) / E11 = (20-15)2/15 = 1.667
-	En calculant pas à pas, on obtient alors des valeurs qu’on peut sommer : 
			1.6667+3.2143+0.8333+1.6667+3.2143+0.8333=11.43

On compare ensuite la valeur obtenue à une valeur seuil de la loi du Khi² avec un certain nombre de degrés de liberté (ddl). Ddl = (nb lignes−1)×(nb colonnes−1) | ddl=(2−1)×(3−1)=1×2=2
Ici on compare à la loi de Khi-deux à 2 dégrés de liberté : 5.99 et on a 11.43 qui est bien supérieur à 5.99 donc on rejette H0 → Il y a indépendance entre l’âge et le type de logement choisi.
L’agence peut personnaliser ses recommandations : lofts et appart' pour les jeunes, maisons pour les familles.





