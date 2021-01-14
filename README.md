# bon_a_python

## ligne de code a ajouter pour transformer une colone de html_recette.csv(fichier test) en soup : 
df['colone'] = df['colone'].apply(BeautifulSoup) 


## code d'import et transformation en soup pour le fichier html_all.csb (1000 recettes) 
df_recette_all = pd.read_csv(link_git_all, index_col=0)
df_recette_all.dropna(inplace=True)
df_recette_all['fiche_recette'] = df_recette_all['fiche_recette'].apply(BeautifulSoup)

