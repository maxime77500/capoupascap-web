# Cap ou pas cap — Site web

Site institutionnel de l'app **Cap ou pas cap** :

- `/` — Landing
- `/privacy` — Politique de confidentialité
- `/support` — Contact / FAQ
- `/reset-password` — Réinitialisation du mot de passe (deep link Supabase)
- `/mentions-legales` — Infos éditeur

## Stack

- HTML / CSS / JS vanilla (pas de framework)
- Hébergé sur Vercel (déploiement automatique sur push main)
- Domaine : capoupascap.app
- Reset password : intégration Supabase JS via CDN

## Points de configuration manuels

1. **Reset password — clé Supabase** : dans public/reset-password.html, remplacer SUPABASE_ANON_KEY_ICI par la clé anon publique.
2. **Privacy Policy — embed Termly** : dans public/privacy.html, remplacer le bloc entre DEBUT TERMLY et FIN TERMLY.
3. **Mentions légales — infos éditeur** : dans public/mentions-legales.html, remplir les champs entre crochets.
4. **Email support / contact** : alias support@capoupascap.app via ImprovMX ou OVH.
5. **Supabase redirect URL** : ajouter https://capoupascap.app/reset-password dans Dashboard → Auth → URL Configuration.
6. **ForgotPasswordScreen côté app** : pointer le redirectTo vers https://capoupascap.app/reset-password.

## Licence

© 2026 Cap ou pas cap.
