# last_test
Tu es un expert en développement web front-end et en design UI/UX.

Je veux créer mon site portfolio personnel en UN SEUL fichier index.html
(HTML + CSS + JavaScript vanilla, zéro framework).

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📋 MES INFORMATIONS PERSONNELLES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Prénom          : [Abel]
Nom             : [KPOKOUTA]
Métier          : [Développeur Full Stack et IA]
Titres animés   : [Le code , c'est nous . Passionné de Tech . Architecte de l'internet]
Phrase accroche : [L'anonymat est mon ancre]
Bio             : [Je suis dev web, IA et aussi youtubeur : creacteru de video suir ma chaine codeavecabel]
Email           : [kpokoutaabel@gmail.com]
Localisation    : [Abomey,BENIN]
GitHub          : [https://github.com/Abel-Dev-KPOKOUTA]
LinkedIn        : [https://www.linkedin.com/in/abel-kocou-kpokouta-6a388739a]
Twitter/X       : []
Photo           : [photo.png]

Chiffres clés :
  - Stat 1 : [EX: 100 → Projets réalisés]
  - Stat 2 : [EX: 3  → Années d'expérience]
  - Stat 3 : [EX: 1200 → Cafés bus ☕]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🛠️ MES COMPÉTENCES (avec niveau en %)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Langages   : [EX: JavaScript 95%, Python 80%, HTML/CSS 98% , PHP 70% , MATLAB 90% , C 80% ]
Frameworks : [EX: DJANGO 98%, CodeIngniter 88%, TailwindCSS 90% ,  FLASK 80% , Scikit-Learn 100% ]
Outils     : [EX: Git/GitHub 95%, Docker 78%, Figma 82%, Supabase 85%, Claude AI 90% , Grok-Automation , Excel , Word , LATEX , ]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🚀 MES PROJETS (3 projets)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Projet 1 :
  - Nom          : [ANONTCHIGAN]
  - Description  : [ANONTCHIGAN est née de la volonté de combiner l'intelligence artificielle et la sensibilisation médicale pour sauver des vies. Notre plateforme offre un accès gratuit à l'information, au dépistage précoce et au soutien pour toutes les femmes.]
  - Technologies : [Python Django, HTML, CSS , JAVASCRIPT, Seaklearn , pandas , tensoflow]
  - GitHub       : [https://github.com/Abel-Dev-KPOKOUTA/anontchigan.git]
  - Demo         : []

Projet 2 :
  - Nom          : [EPreuvePro]
  - Description  : [Gestion des epreuves dans un groupe de professeurs et favorisée l'acces à tous des ressources pour etudier .  Plateforme éducative béninoise de partage d'épreuves et corrigés - BEPC & BAC | Django | FedaPay | 2500+ épreuves | 15K+ élèves]
  - Technologies : [Python]
  - GitHub       : [https://github.com/Abel-Dev-KPOKOUTA/epreuvespro.git]
  - Demo         : []

Projet 3 :
  - Nom          : [Bibliotheque en Ligne]
  - Description  : [Gestion des bibliotheQUES EN LIGNE]
  - Technologies : [PHP Framework codeigniter , HTML, CSS , CPANEL]
  - GitHub       : [https://github.com/Abel-Dev-KPOKOUTA/Digital-Library-Manager.git]
  - Demo         : []

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🗄️ CONNEXION SUPABASE (OBLIGATOIRE)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SUPABASE_URL  : [EX: https://xxxx.supabase.co]
SUPABASE_ANON : [TA CLÉ PUBLIQUE anon/publishable]

Le formulaire de contact DOIT :
  1. Charger le SDK Supabase via CDN AVANT tout autre script :
       <script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>

  2. Initialiser le client exactement comme ceci :
       const { createClient } = supabase;
       const db = createClient(SUPABASE_URL, SUPABASE_ANON);

  3. Au submit, insérer dans la table "contact_messages" avec ces colonnes :
       { name, email, subject, message }
       via : await db.from('contact_messages').insert([{...}])

  4. Gérer les erreurs : afficher alert() avec error.message si échec

  5. En cas de SUCCÈS :
       - NE PAS faire contactForm.style.display = 'none' (ça casse l'affichage)
       - Faire à la place :
           document.querySelectorAll('.form-group, .form-row, .btn-submit')
             .forEach(el => el.style.display = 'none');
       - Puis afficher le div#formSuccess qui est DANS le form
       - Puis scroller dessus avec scrollIntoView()

  Le SQL à exécuter dans Supabase pour créer la table et autoriser les INSERT :
  
       CREATE TABLE IF NOT EXISTS contact_messages (
         id         uuid DEFAULT gen_random_uuid() PRIMARY KEY,
         name       text NOT NULL,
         email      text NOT NULL,
         subject    text NOT NULL,
         message    text NOT NULL,
         created_at timestamptz DEFAULT now()
       );

       ALTER TABLE contact_messages ENABLE ROW LEVEL SECURITY;

       CREATE POLICY "Allow public insert"
       ON contact_messages
       FOR INSERT
       TO anon
       WITH CHECK (true);

  Inclure ce bloc SQL en commentaire dans le fichier HTML pour référence.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🎨 DESIGN
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- Fond          : #0a0a0f (noir profond)
- Accent        : #7c3aed (violet)
- Texte         : blanc cassé
- Font titres   : Google Fonts "Syne"
- Font corps    : Google Fonts "DM Sans"
- Design        : minimaliste, épuré, beaucoup d'espaces
- 100% responsive (mobile, tablette, desktop)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📐 SECTIONS À GÉNÉRER (dans cet ordre)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
1. NAV fixe avec effet blur au scroll + menu hamburger mobile
2. HERO avec typing effect animé sur le titre de poste
3. À PROPOS avec photo ronde (fichier: [NOM IMAGE]) + bio + 3 stats animées
4. COMPÉTENCES en 3 catégories avec barres de progression animées
5. PROJETS en grille 3 cartes avec overlay violet au hover
6. CONTACT avec formulaire Supabase connecté (voir section ci-dessus)
7. FOOTER avec nom, année dynamique, icônes GitHub / LinkedIn / Twitter

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
⚙️ RÈGLES TECHNIQUES STRICTES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- Tout dans UN SEUL fichier index.html
- CSS custom properties pour toutes les couleurs et espacements
- Animations scroll via Intersection Observer API
- Animations CSS avec keyframes
- JavaScript vanilla uniquement, aucun framework
- Commentaires clairs dans le code pour chaque section
- INTERDIT : balise </script> orpheline en fin de fichier
- INTERDIT : cacher le <form> entier pour afficher le succès
- Code propre, bien indenté, prêt pour GitHub Pages
- Le SDK Supabase doit être chargé AVANT le script principal
