# Aplicație Client HTTP pentru UtmShop

## Descriere
Această aplicație implementează un client HTTP care interacționează cu API-ul magazinului online UtmShop. 

### Componente server
Instalam .NET SDK și runtime:
   ```bash
   brew install --cask dotnet-sdk
   ```
 Instalam Runtime-ul .NET 5.0 de pe site-ul oficial Microsoft

### Pornire server
Pentru a porni serverul API, navigați în directorul proiectului și rulați:
```bash
dotnet restore
dotnet build
dotnet run
```

Verificați că serverul funcționează accesând Swagger UI:
```
https://localhost:5001/swagger/index.html
```

### Configurare client
1. Instalați bibliotecile Python necesare:
   ```bash
   pip install requests urllib3
   ```
2. Salvati fișierul `client_magazin.py` în directorul dorit

## Funcționalități implementate

Clientul implementează toate cerințele specificate în laborator:

1. **Listarea categoriilor** - Afișează toate categoriile disponibile
2. **Detalii despre o categorie** - Afișează informații complete despre o categorie
3. **Crearea unei categorii noi** - Adaugă o categorie cu titlu și descriere
4. **Ștergerea unei categorii** - Elimină o categorie existentă din sistem
5. **Modificarea titlului unei categorii** - Actualizează numele unei categorii
6. **Listarea produselor dintr-o categorie** - Afișează toate produsele dintr-o categorie
7. **Adăugarea unui produs nou** - Creează un produs nou cu nume, descriere, preț și stoc

## Utilizare

Rulați aplicația client:
```bash
python client_magazin.py
```
