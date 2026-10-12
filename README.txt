Kurmanji Adventure 5.0 - kontopilot

Detta ar en separat pilot, inte en ersattning av befintligt spel.
Innehall: index.html med vuxenregistrering, login, testbarnprofiler och lasning av XP.
Krav: befintliga Supabase-tabeller ka_children, ka_guardians och ka_progress med RLS.

Publicering: skapa ett nytt PUBLIC GitHub-repository (t.ex. kurmanji-adventure-pilot),
ladda upp index.html och aktivera GitHub Pages (main / root).
OBS: Uppdatera Supabase Auth Redirect URLs med pilotens EXAKTA GitHub Pages-adress.
Vid behov ange pilotadressen som Site URL for pilotprojektet.

VIKTIGT: Anvand ENDAST TESTDATA. Ingen verklig elevinformation.
RLS ar inte penetrationstestat. Den befintliga progress-policyn tillater
klientskrivning av XP och ska hardas innan spelintegration.
Ingen lararroll finns annu. Testa tva vuxenkonton och kontrollera att
vuxen A inte kan lasa vuxen B:s barnprofiler.
Gamla framsteg migreras INTE automatiskt. Spara backup via befintliga spelet.
Ingen secret/service_role key ska laggas i denna statiska app.
