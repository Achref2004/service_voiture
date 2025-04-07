<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Location </title>
    <link rel="stylesheet" href="front.css">
    
</head>
<body>
  <!-- Section Véhicules -->
    <section id="vehicules" class="section">
        <div class="container">
            <h2 style="color: rgba(4, 6, 117, 0.84);">Notre Collection</h2>
            <div class="cars-grid">
                <!-- Voitures ajoutées dynamiquement -->
            </div>
        </div>
    </section>

</body>

<script>

<script>
        const cars = [
            {
                name: "MERCEDES",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/92a77764-235c-439b-9e38-1b612d9c1296/bf74d17d-1720-40a0-b838-237699046743.png",
                price: "100 DT/jour💸",
                dispo: "Disponible ",
                transmission: "Automatique",
                year: "2025"
            },
            {
                name: "KIA",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/039e7e14-e834-4f38-afdc-92531295fa27/cde9a737-de3e-437f-a355-6b63f88a6e23.png",
                price: "70 DT/jour💸",
                dispo: "dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
            {
                name: "KIA RIO",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/9cf5740b-f15a-454e-8bf5-5641a3b187f3/1757c04e-7a55-44e5-98c9-4695d24dc34a.png",
                price: "70 DT/jour💸",
                dispo: "Non Disponible ",
                transmission: "Automatique",
                year: "2025"
            },
            {
                name: "BMW",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/b28e5f74-f33b-43c3-8515-da84c540c6c0/f097a881-9e75-4ece-8284-46efac1bf075.png",
                price: "100 DT/jour💸",
                dispo: "dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
            {
                name: "POLO",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/c82b1492-8e23-4469-a701-c4ce73b9b380/9a6f9eed-c4a8-418d-9f34-db7076d23c4d.png",
                price: "100 DT/jour💸",
                dispo: "dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
            {
                name: "GOLF 7 ",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/56982fbc-4b46-420a-a5fa-f0dbb285ac40/819323ec-34d3-49a5-bc90-3acb5623ba21.png",
                price: " --DT/jour💸",
                dispo: "non dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
            {
                name: "NISSANE",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/9d848a14-716f-4ff6-bd5e-abdd4ab82d81/bdea306f-0d49-439e-8aa5-39daa3247826.png",
                price: "70 DT/jour💸",
                dispo: "dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
            {
                name: "MERCEDES",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/f8b8372f-2f47-4bdf-b10c-ae1c496ab07d/c0d415aa-3368-4081-a2ed-8607fbacba0d.png",
                price: "100 DT/jour💸",
                dispo: "Disponible ",
                transmission: "Automatique",
                year: "2025"
            },
         
            {
                name: "BMW classique ",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/28205749-8953-444b-969e-9d2fbaf9dab3/c71b44a1-422e-4d8f-bbb6-de19a6b779ed.png",
                price: " --DT/jour💸",
                dispo: "non dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
        
            {
                
                name: "CLIO ",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/6c49dab1-4c67-4854-9782-79028a8afba0/26436527-84c7-435e-856c-6f6893e599a4.png",
                price: " --DT/jour💸",
                dispo: "non dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
        
            {
                name: "TOYOTA CORELLA HIAS ",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/6c49dab1-4c67-4854-9782-79028a8afba0/26436527-84c7-435e-856c-6f6893e599a4.png",
                price: " --DT/jour💸",
                dispo: "non dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
        
            {
                name: "Marcedess classique ",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/6c49dab1-4c67-4854-9782-79028a8afba0/26436527-84c7-435e-856c-6f6893e599a4.png",
                price: " --DT/jour💸",
                dispo: "non dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
        
            {
                name: "Marcedess classique ",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/6c49dab1-4c67-4854-9782-79028a8afba0/26436527-84c7-435e-856c-6f6893e599a4.png",
                price: " --DT/jour💸",
                dispo: "non dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
        
            {
                name: "WALIS ",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/6c49dab1-4c67-4854-9782-79028a8afba0/26436527-84c7-435e-856c-6f6893e599a4.png",
                price: " --DT/jour💸",
                dispo: "non dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
        
            {
                name: "RENAULT 21 ",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/6c49dab1-4c67-4854-9782-79028a8afba0/26436527-84c7-435e-856c-6f6893e599a4.png",
                price: " --DT/jour💸",
                dispo: "non dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
            {
                name: "SYMBOL ",
                image: "https://cdn.qwenlm.ai/output/23d6bba8-9bd4-43b6-9bdd-3082a904b658/t2i/6c49dab1-4c67-4854-9782-79028a8afba0/26436527-84c7-435e-856c-6f6893e599a4.png",
                price: " --DT/jour💸",
                dispo: "non dsiponible",
                transmission: "Automatique",
                year: "2025"
            },
        
        
            
        ];

    </script>