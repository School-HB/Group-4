# 📅 School-Hub - Gestion des Présences

**Portail de suivi et contrôle de l'assiduité des élèves**

---

## 📋 À propos

Portail de **Gestion des Présences** du système School-Hub pour le suivi de l'assiduité scolaire.

**Fonctionnalités** :
- Pointage quotidien des élèves
- Suivi des absences et retards
- Rapports statistiques
- Gestion des justificatifs

---

## 🔧 Prérequis

- PHP >= 8.1
- Composer >= 2.5
- Node.js >= 18.x
- npm ou yarn
- SQLite >= 3.x

---

## 📁 Structure

```
Group-4/
├── backend/              # API Laravel
│   ├── database/
│   │   └── database.sqlite
│   └── .env
├── frontend/             # Interface React
│   └── src/
└── README.md
```

---

## 🚀 Installation

### 1. Cloner le projet

```bash
git clone https://github.com/School-HB/Group-4.git
cd Group-4
```

### 2. Backend (Laravel)

```bash
cd backend

# Installer les dépendances
composer install

# Copier la configuration
cp .env.example .env

# Créer la base de données SQLite
touch database/database.sqlite

# Exécuter les migrations et seeders
php artisan migrate --seed

# Démarrer le serveur
php artisan serve --port=8001
```

✅ Backend : `http://localhost:8001`

### 3. Frontend (React)

```bash
cd frontend

# Installer les dépendances
npm install

# Créer le fichier .env
echo "VITE_API_URL=http://localhost:8001/api" > .env

# Démarrer le serveur
npm run dev
```

✅ Frontend : `http://localhost:5173`

---

## 🎯 Démarrage

**Terminal 1 - Backend :**
```bash
cd backend
php artisan serve --port=8001
```

**Terminal 2 - Frontend :**
```bash
cd frontend
npm run dev
```

---

## 👤 Comptes de test

| Rôle | Email | Mot de passe |
|------|-------|--------------|
| Admin | admin@school-hub.com | password |
| Surveillant | surveillant@school-hub.com | password |
| Enseignant | teacher@school-hub.com | password |

---

## 🛠️ Commandes utiles

### Backend
```bash
# Réinitialiser la DB
php artisan migrate:fresh --seed

# Nettoyer le cache
php artisan cache:clear
php artisan config:clear
```

### Frontend
```bash
# Build de production
npm run build

# Linter
npm run lint
```

---

## 👥 Équipe

Développé par **Group-4**

---

## 📄 License

MIT License