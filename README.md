# 📚 Book Library Management System

![Project Logo](https://arvja.no/img/nkey.jpg)

## 📝 Om prosjektet
Dette er et **ASP.NET Core MVC-prosjekt** for et bibliotekssystem som bruker **SQLite** som database. Det lar deg **legge til, redigere, slette, forhåndsvise og laste ned bøker**. Alle bøker har en **bokomslags-URL** og en **lenke til en TXT-fil**.

---

# 🚀 **Hvordan laste ned og kjøre prosjektet**

## **1️⃣ Klon prosjektet fra GitHub**
Åpne terminalen eller **Git Bash** og kjør:
```sh
 git clone https://github.com/DITT-BRUKERNAVN/BookLibraryManagement.git
```
Deretter, gå inn i prosjektmappen:
```sh
 cd BookLibraryManagement
```

## **2️⃣ Åpne prosjektet i Visual Studio**
1. **Åpne Visual Studio 2022**.
2. Klikk **"Open a project or solution"**.
3. Finn `BookLibraryManagement.sln` og åpne det.

---

## **3️⃣ Installer nødvendige avhengigheter**
Før du kjører prosjektet, må du installere **NuGet-pakkene**.

### 📦 **Installer pakkene**
Åpne **Package Manager Console** (`Tools` → `NuGet Package Manager` → `Package Manager Console`) og kjør:
```powershell
 dotnet restore
```
Dette laster ned alle nødvendige avhengigheter, inkludert **Entity Framework Core** og **SQLite**.

---

## **4️⃣ Sjekk at databasen eksisterer**
Prosjektet bruker **SQLite**, og databasen skal være inkludert i mappen. Slik sjekker du:
1. **Gå til prosjektmappen**.
2. **Se etter filen `BookLibrary.db`** i `Data`-mappen.

### ❌ **Hvis databasen mangler, opprett den med disse kommandoene:**

Åpne **Package Manager Console** og kjør:
```powershell
Add-Migration InitialCreate
Update-Database
```
Dette vil **generere databasen og opprette tabellene**.

---

## **5️⃣ Kjør prosjektet** 🚀
Når alt er klart, kjør prosjektet:
```sh
 dotnet run
```
Eller, i **Visual Studio**:
1. Klikk **"Start" (Ctrl + F5)**.
2. Nettleseren åpner seg, og du ser **bibliotekssystemet ditt**.

---

# ✅ **Prosjektfunksjoner**
- **CRUD-funksjonalitet** (Legge til, redigere, slette bøker).
- **Bootstrap 5-design** for en ren og brukervennlig UI.
- **SQLite-database** for enkel datahåndtering.
- **Håndtering av bokomslag og TXT-nedlastinger**.
- **Referanse til Project Gutenberg for bøker**.

🔗 **Nettside for bøker:** [Project Gutenberg](https://www.gutenberg.org/)

---

# 📌 **Hvordan bidra?**
1. **Fork prosjektet på GitHub**.
2. **Lag en ny branch** for dine endringer:
   ```sh
   git checkout -b feature-navn
   ```
3. **Gjør endringer og commit**:
   ```sh
   git commit -m "La til ny funksjonalitet"
   ```
4. **Push endringene til GitHub**:
   ```sh
   git push origin feature-navn
   ```
5. **Opprett en Pull Request (PR)** på GitHub.

---

# 🛠 **Feilsøking**
### 🔴 **Prosjektet kjører ikke?**
- Sørg for at **NuGet-pakkene er installert** (`dotnet restore`).
- Sjekk om **`BookLibrary.db` eksisterer**.
- Hvis databasen mangler, kjør:
  ```powershell
  Update-Database
  ```

### 🔴 **Kan ikke laste ned bøker?**
- Sjekk at `PdfUrl` i databasen peker til en gyldig `.txt`-fil.
- Test en fungerende lenke, f.eks.:  
  ```
  https://www.gutenberg.org/files/1342/1342-0.txt
  ```

---

# 🏆 **Takk for at du bruker Book Library Management System!** 🎉
