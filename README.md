# Demos libcna.com

Statický web s ukázkami postavenými nad **libcna**. Každá ukázka je samostatný
WebAssembly build; úvodní stránka slouží jako jejich rozcestník.

## Ukázky

- **CNA Craft** – `cna-craft/CnaCraft.html`
- **CNA Examples** – `cna-examples/cna_examples.html`
- **Mesh Craft** – `mesh-craft/MeshCraft.html`
- **2D demo** – `cna_demo_2d/cna_demo_2d.html`
- **3D House demo** – `cna_demo_house_3d/cna_house3d_demo.html`
- **Black Pine** – `black-pine/black-pine.html`
- **Iron Gang** – `iron-gang/play.html`
- **Lines CNA** – `lines-cna/winlinez_cna.html`
- **Copper Boots** – `mario-cna/copper-boots.html`
- **People** – `people-cna/People.html`
- **Tamagotchi CNA** – `tamagotchi-cna/TamagotchiCna.html`
- **Wolf CNA** – `wolf-cna/wolf-cna.html`
- **CNA Car Simulator** – `cna-car-simulator/cna-car-simulator.html`
- **CNA Street** – `cna-street/cna-street.html`
- **Living Room Simulator** – `living-room-simulator/living-room-simulator.html`

## Lokální spuštění

Kvůli načítání souborů `.wasm` a `.data` web neotevírejte přímo ze souborového
systému. Spusťte v kořeni projektu jednoduchý HTTP server:

```bash
python3 -m http.server 8000
```

Poté otevřete [http://localhost:8000](http://localhost:8000).

## Nasazení

Projekt nevyžaduje sestavovací krok. Na statický hosting nahrajte celý obsah
repozitáře a jako výchozí dokument použijte `index.html`. Server musí pro
WebAssembly vracet MIME typ `application/wasm`.
