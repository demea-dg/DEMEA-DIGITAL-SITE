DEMEA DIGITAL GROWTH — SITE WEB (VERSION DE PREPARATION)

FICHIERS
- index.html : site principal
- assets/demea-logo.png : logo
- mentions-legales.html : trame à compléter après immatriculation
- confidentialite.html : trame à compléter et valider
- merci.html : page de confirmation du formulaire

FORMULAIRE
Le formulaire est préparé pour Netlify Forms (nom : contact-demea), avec champ anti-spam et page de confirmation.
Après déploiement : ouvrir le site dans Netlify > Forms, activer la détection des formulaires si demandé, puis envoyer un formulaire test.
Pour recevoir les demandes par email : Netlify > Forms > Submission notifications > Add notification. Le destinataire doit être un membre actif de l'équipe Netlify.

AVANT PUBLICATION COMMERCIALE
1. Créer et immatriculer l'entreprise via https://formalites.entreprises.gouv.fr/.
2. Vérifier le nom commercial / la marque DEMEA et les activités déclarées.
3. Enregistrer demeadigital.fr après vérification Whois Afnic et recherche de marque INPI.
4. Créer et tester contact@demeadigital.fr chez le fournisseur email choisi.
5. Déployer le dossier sur Netlify et connecter le domaine avec les DNS fournis par Netlify.
6. Compléter les mentions légales avec identité, forme, adresse, SIREN et hébergeur exacts.
7. Finaliser la politique de confidentialité : responsable, outils/sous-traitants, transferts éventuels, conservation, contact et droits.
8. Configurer les notifications du formulaire, tester mobile/ordinateur et vérifier les emails reçus.

IMPORTANT
Cette version est une préparation technique, pas un site juridiquement prêt à publier. Les pages légales contiennent volontairement des champs à compléter. Le formulaire ne fonctionnera qu'après déploiement Netlify, activation de la détection et configuration des notifications. L'adresse contact@demeadigital.fr est une adresse prévue, pas encore créée ni vérifiée.

OFFRES ACTUELLES : DEMEA Starter 80 € au lieu de 180 € ; DEMEA Business 424,15 € au lieu de 499 € (−15 %) ; DEMEA Automation 594,15 € au lieu de 699 € (−15 %). Abonnements facultatifs : Maintenance Essentielle 29 €/mois, DEMEA Visibility 59 €/mois, Maintenance Plus 89 €/mois. Prix indicatifs à contractualiser précisément. Hébergement, domaine, licences et services tiers exclus sauf mention contraire au devis.


CHATBOT IA DEMEA (V8)
- Widget de discussion intégré au site, avec réponses naturelles via l'API OpenAI Responses.
- Fonction serveur : netlify/functions/chat.js. La clé API n'est jamais exposée dans le navigateur.
- Capture de prospects via Netlify Forms (formulaire chatbot-leads).

MISE EN SERVICE OBLIGATOIRE SUR NETLIFY
1. Déployer le dossier DEMEA-site (ou son contenu) sur Netlify.
2. Dans Site configuration > Environment variables, ajouter OPENAI_API_KEY avec votre clé API OpenAI. Ne jamais coller cette clé dans index.html ni dans un message public.
3. Facultatif : définir OPENAI_MODEL (par défaut gpt-5.5).
4. Activer la détection des formulaires Netlify puis redéployer le site.
5. Dans Forms > Notifications, configurer l'adresse email qui doit recevoir les nouvelles demandes du formulaire chatbot-leads et tester une soumission.
6. Tester une conversation sur le site publié et vérifier les logs de la fonction si nécessaire.

IMPORTANT
- Le chatbot ne peut répondre avec l'IA qu'après configuration de OPENAI_API_KEY et déploiement de la fonction serveur.
- Les demandes de rappel sont enregistrées via Netlify Forms ; les notifications email doivent être configurées dans le tableau de bord Netlify.
- Les frais d'utilisation de l'API OpenAI sont facturés séparément selon le compte et l'usage.
- Avant mise en production, compléter les mentions légales et la politique de confidentialité, informer les visiteurs du traitement de leurs messages et coordonnées, définir une durée de conservation et vérifier les réglages RGPD/Netlify/OpenAI.
