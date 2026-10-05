# Anis — portfolio

## Projets

| Dépôt | Description | Stack |
|---|---|---|
| [extrabat](https://github.com/anis-dev-portfolio/extrabat) | SaaS multi-tenant de suivi de chantier pour le BTP, avec abonnement Stripe. En production. | Next.js · Supabase · Prisma · Stripe |
| [asas-voice](https://github.com/anis-dev-portfolio/asas-voice) | Dictée vocale desktop : transcription et correction par IA. | Tauri (Rust) · React · Fastify · Mistral · Claude |

Également en ligne, code non partagé : [weydaa.com](https://weydaa.com) (petites annonces, fr/ar/en) · [mt-structura.fr](https://www.mt-structura.fr) · [iso-bat.com](https://www.iso-bat.com).

## Par où commencer

- **extrabat** — [README](https://github.com/anis-dev-portfolio/extrabat/blob/main/README.md) · [SECURITY](https://github.com/anis-dev-portfolio/extrabat/blob/main/SECURITY.md) · abonnement : [`lib/abonnement-stripe.ts`](https://github.com/anis-dev-portfolio/extrabat/blob/main/lib/abonnement-stripe.ts), [`app/api/stripe/webhook/route.ts`](https://github.com/anis-dev-portfolio/extrabat/blob/main/app/api/stripe/webhook/route.ts) · règles du projet : [`CLAUDE.md`](https://github.com/anis-dev-portfolio/extrabat/blob/main/CLAUDE.md)
- **asas-voice** — [README](https://github.com/anis-dev-portfolio/asas-voice/blob/main/README.md) · [SECURITY](https://github.com/anis-dev-portfolio/asas-voice/blob/main/SECURITY.md) · backend et appels aux modèles : [`apps/backend/src/routes/`](https://github.com/anis-dev-portfolio/asas-voice/tree/main/apps/backend/src/routes)

Statut, mesures de sécurité et limites connues sont détaillés dans le README et le SECURITY.md de chaque dépôt.

## Méthode

Développement assisté par IA (Claude Code), encadré : invariants par projet dans `CLAUDE.md`, travail par phases, typecheck et lint avant chaque livraison.

```bash
# extrabat
npm install && npm run lint && npm run build

# asas-voice
pnpm install && pnpm typecheck && pnpm lint && pnpm test
```

---

Dépôts privés. Code propriétaire, tous droits réservés. Accès en lecture accordé uniquement à des fins d'évaluation.
