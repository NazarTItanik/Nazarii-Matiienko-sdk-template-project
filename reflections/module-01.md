# Module 1 — Reflection

## What I did

Copied `.env.example` to `.env` (ports and database credentials), started the
stack with `docker compose up --build` and checked that all six containers came
up and `/products`, `/users` and `/orders` returned `200`. After that I opened
`http://localhost:5173/` to check visually that the page loaded and showed the
products, users and orders. Then I drew my own system map in
draw.io, traced `GET /products` from the frontend to the database and back, and
compared the docs with the code.

## What I did not understand at first

I thought the frontend container calls the backend services, as the diagram in
`ARCHITECTURE.md` shows. In fact it only serves the JS files, and the browser
calls the services on `localhost`. I also thought the migration runner runs only
on the first launch, but it runs on every `docker compose up` and then exits.

## What I would do differently

I would go through the files fully understanding the task instead of rushing into code and reading it from the code perspective. It is the way more easier to read the code when you know the structure. Also, I would simply use Network section in Dev Tools to analyze which requests are made (when examining from above, not code itself to faster grasp connections). 

## How long this took me

The first build took about 6–7 minutes; the whole module took about 2-3 hours.
