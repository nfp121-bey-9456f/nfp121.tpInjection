# exemple extrait du support, NFP121, injection de dépendances
# exemples des possibilités syntaxiques du fichier de config 
#verbose=true

# un bean avec 'a' comme indentifiant
bean.id.1=a
# bean instance de cette classe
a.class=syntaxe_exemples.A
# attribut i
a.property.1=i
#appel de setI(b)
a.property.1.param.1=b
# attribut f
a.property.2=f
# appel de setF(3.154)
a.property.2.param.1=3.154
# attribut tab
a.property.3=tab
# appel de setTab(new in[]{3, 54, 4, 6, 7})
a.property.3.param.1=3 54 4 6 7
a.property.4=ti
a.property.4.param.1=b b1 b b1

# un bean avec 'b' comme indentifiant
bean.id.2=b
b.class=syntaxe_exemples.B

# un bean avec 'b1' comme indentifiant
bean.id.3=b1
b1.class=syntaxe_exemples.B1

# un bean avec 'uneTable' comme indentifiant
bean.id.4=uneTable
uneTable.class=syntaxe_exemples.Table
# attribut collection
uneTable.property.1=collection
# appel de setCollection(liste)
uneTable.property.1.param.1=liste
# attribut int
uneTable.property.2=int
# apple de setInt(3)
uneTable.property.2.param.1=3
uneTable.property.3=int
uneTable.property.3.param.1=4

bean.id.5=liste
liste.class=java.util.HashSet

bean.id.6=fabrique
fabrique.class=syntaxe_exemples.Factory
fabrique.property.1=instance
#fabrique.property.1.param.1=java.util.TreeSet.class
fabrique.property.1.param.1=java.util.HashSet.class

bean.id.7=listeDeTables
listeDeTables.class=syntaxe_exemples.ListeDeTables
listeDeTables.property.1=table
listeDeTables.property.1.param.1=uneTable
listeDeTables.property.2=tables
listeDeTables.property.2.param.1=uneTable uneTable uneTable

#bean.id.8=gui
#gui.class=config_editor.GUI
