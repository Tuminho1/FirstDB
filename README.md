# FirstDB
Questa immagine mostra cosa succede nel terminale quando si va a creare un nuovo progetto su Visual Studio utilizzando Dotnet new console

![image](https://user-images.githubusercontent.com/116791499/236140188-f70ebbf9-1bab-4595-a2c2-effa319e7c6a.png)
__________________________________________________________________________________________________

Ecco l'estensione da cercare su Visual Studio Code per trovare i comandi da aggiungere per includere la libreria sqlite-net-pcl

![image](https://user-images.githubusercontent.com/116791499/236141827-0368fb33-3d6b-414f-acba-8a4cefb9d43e.png)
__________________________________________________________________________________________________

Qui sotto troviamo il link con collegameto al download per scaricare il diagramma relazionale del db chinook.db

https://www.sqlitetutorial.net/sqlite-sample-database/#:~:text=the%20following%20link.-,Download%20SQLite%20sample%20database,-In%20case%20you

using SQLite;
__________________________________________________________________________________________________

## il codice C# necessario per visualizzare il codice  chinook.db:

Console.WriteLine("Hello World");

SQLiteConnection cnl = new SQLiteConnection("chinook.db");

var tblArtist = cnl.Query<Artist>("select * from artists");

Console.WriteLine( $"In questa tabella ci sono {tblArtist.Count} record!");

public class Artist+

{

    public int ArtistId{get; set;}
    
    public string Name{get; set;}
    
}

![image](https://user-images.githubusercontent.com/116791499/236138255-9ac49b27-8871-4ccd-a50c-cb0f57baae54.png)
