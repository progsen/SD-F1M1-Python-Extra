# Map en Github repository maken voor Python Extra

Voor de opdrachten en code die je maakt voor de Python Extra lessen maak je een map aan op je computer. Deze map koppel je aan een nieuwe Github repository voor Python Extra

1. Elke week maak je een nieuwe map **met een duidelijke naam** in de hoofdmap
2. Al je werk maak je in die map
3. Aan het einde van de les **commit** en **push** je alle wijzigingen naar je Github.

**Hieronder staat hoe je die map en Github repository aanmaakt.En hoe je  de code er in zet, commit en pusht.**

---

### 1. Map maken: Flex-PythonExtra

Ga naar de plek waar je de map wil en maak daar de map *"Flex-PythonExtra"*

![](map-pythonextra.png)

---

### 2. Nieuwe Github repository maken
Login op Github en klik op "New repository"

![](new_repository.png)

Vul de gegevens als volgt in, met jouw naam en klas en **selecteer de optie om een README.me bestand te maken**. Klik dan op "Create repository":

![](create_repo.png)

---

### 3. Git repository maken op je computer
Ga naar de map **Flex-PythonExtra** en open daar een Powershell/Command venster (Windows) en als je op een Mac werkt een [Terminal venster](mac_terminal){:target="_blank"}.

Zorg dat je in de **Flex-PythonExtra** map staat en *initialiseer een nieuwe Git repository* met het volgende commando:

```bash
git init
```

![](git_init.gif)

---

### 4. Kopieer de URL van je Github repository
Ga naar je Github repository en kopieer de **HTTPS** url onder de Code knop:

![](github_copy_url.gif)

---

### 5. Github repository koppelen aan de Git repository op je computer
Met het commando `git remote add origin <URL>` koppel je je Github repository aan de map op je computer. Bij `<URL>` plak je de url die je in stap 4 hebt gekopieerd.

![](git_remote_add.gif)

Je kunt controleren of het gelukt is met het commando: 

```bash
git remote -v
``` 

Dit laat zien welke externe Git repository (Github) aan je lokale repository (op je computer) is gekoppeld.

---

### 6. De laatste wijzigingen van Github halen
Nu de map goed is gekoppeld kun je alle wijzigingen die je nog niet hebt, ophalen van Github. Want (weet je nog) je hebt een README.md bestand gemaakt.

Voer nu dit commando uit:

```bash
git pull origin main
```

![](git_pull_origin_master.gif)

Hiermee haal je de `main` branch op naar je computer (de `main` is de standaard branch in Git)

**Als het goed is heb je nu het README.md bestand op je computer staan**

---

### 7. README bestand wijzigen
Je gaat nu een wijziging doen aan het `README.md` bestand.  
Open het bestand `README.md` in kladblok, of een andere tekst editor en zet jouw naam en klas er in en bewaar het bestand.

![](readme_edit.gif)

---

### 8. De wijzigingen opsturen naar Github
Nu kun je jouw wijzigingen **committen** en **pushen** naar Github. 

* Eerst kijk je met `git status` wat de wijzigingen zijn. 
* Dan selecteer je alle wijzigingen met `git add .` 
* Nu commit je alles: `git commit -m "README gewijzigd"`
* Wijzigingen naar Github *pushen*: `git push -u origin main`

![](git_commit_push.gif)

Kijk nu in je Github repository of je commit en wijziging er staat:

![](check_commit.gif)

---

## Lever je Github URL in 

Als dit allemaal gelukt is, lever dan de Github URL via deze link in:
[Klik hier om je Python Extra Github URL in te leveren]({{ site.flex.form_link }}){:target="_blank" }

> Zo kan ik je helpen, feedback geven en uiteindelijk ook al je werk beoordelen


---

## Eindelijk... aan de slag

[Aan de slag met Turtle graphics](../01-turtle-graphics/index.md){:class="next"}
