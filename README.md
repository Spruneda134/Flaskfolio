# Flaskfolio – Early Personal Website (Archived)

This repository contains one of my early personal website projects, built using **Flask**, **HTML templates**, and simple text-based content loading.  
It served as a practice project while I was learning backend routing, templating, and basic form handling in Python.

This project is no longer maintained, but it remains public as an archive of my early development work.

---

## Project Overview

**Tech Stack:**
- Python  
- Flask  
- Jinja2 Templates  
- Basic static file handling (e.g., `details.txt`)

**Features:**
- Homepage that renders personal details from a text file  
- Dynamic user greeting via route parameters  
- Multiple Flask routes (`/`, `/another`, `/user/<name>`, `/form`)  
- Basic form submission demo  
- Lightweight personal-site structure using templates (`base.html`, `another.html`, `form.html`)

---

## Example Snippet
```python
@app.route("/")
def homePage():
    name = "Salvador Pruneda"
    details = readDetails('static/details.txt')
    return render_template('base.html', name=name, aboutMe=details)
