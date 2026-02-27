import { useState, useEffect, useRef, useCallback, useMemo, createContext, useContext } from "react";

// ═══════════════════════════════════════════════════════════════
// SEOBYRÅ.COM — Norges #1 SEO-kunnskapsplattform
// Full SPA with routing, parallax, custom icons, 15+ pages
// ═══════════════════════════════════════════════════════════════

// ── CUSTOM SVG ICONS ──────────────────────────────────────────
const Icon = {
  Search: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round"><circle cx="10.5" cy="10.5" r="7"/><path d="M21 21l-5.2-5.2"/></svg>
  ),
  Bolt: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><path d="M13 2L4.5 13H12l-1 9 8.5-11H12l1-9z"/></svg>
  ),
  Globe: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5"><circle cx="12" cy="12" r="10"/><ellipse cx="12" cy="12" rx="4" ry="10"/><path d="M2 12h20"/></svg>
  ),
  Code: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
  ),
  Link: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"/><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"/></svg>
  ),
  Chart: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round"><path d="M3 3v18h18"/><path d="M7 16l4-8 4 4 5-9"/></svg>
  ),
  Brain: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><path d="M12 2C8.5 2 6 4.5 6 7.5c0 1.5.5 2.8 1.3 3.8C6.5 12.3 6 13.6 6 15c0 3 2.5 5 5 5h2c2.5 0 5-2 5-5 0-1.4-.5-2.7-1.3-3.7.8-1 1.3-2.3 1.3-3.8C18 4.5 15.5 2 12 2z"/><path d="M12 2v20"/><path d="M8 7h8"/><path d="M7 12h10"/><path d="M8 17h8"/></svg>
  ),
  Shield: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><path d="M12 2l8 4v6c0 5.5-3.8 10.7-8 12-4.2-1.3-8-6.5-8-12V6l8-4z"/></svg>
  ),
  Target: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5"><circle cx="12" cy="12" r="10"/><circle cx="12" cy="12" r="6"/><circle cx="12" cy="12" r="2"/></svg>
  ),
  Layers: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
  ),
  MapPin: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5"><path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7z"/><circle cx="12" cy="9" r="2.5"/></svg>
  ),
  Pencil: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><path d="M17 3a2.83 2.83 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"/></svg>
  ),
  Robot: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><rect x="4" y="8" width="16" height="12" rx="2"/><path d="M12 2v6"/><circle cx="9" cy="13" r="1"/><circle cx="15" cy="13" r="1"/><path d="M9 17h6"/><path d="M2 14h2"/><path d="M20 14h2"/><circle cx="12" cy="2" r="1"/></svg>
  ),
  Gauge: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round"><path d="M12 22c5.5 0 10-4.5 10-10S17.5 2 12 2 2 6.5 2 12s4.5 10 10 10z"/><path d="M12 6v6l4 2"/></svg>
  ),
  Arrow: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><path d="M5 12h14"/><path d="M12 5l7 7-7 7"/></svg>
  ),
  ArrowDown: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><path d="M12 5v14"/><path d="M5 12l7 7 7-7"/></svg>
  ),
  Menu: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round"><path d="M3 6h18M3 12h18M3 18h18"/></svg>
  ),
  X: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round"><path d="M18 6L6 18M6 6l12 12"/></svg>
  ),
  ChevronDown: ({ size = 16, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="2" strokeLinecap="round"><path d="M6 9l6 6 6-6"/></svg>
  ),
  File: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/></svg>
  ),
  Network: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5"><circle cx="12" cy="5" r="3"/><circle cx="5" cy="19" r="3"/><circle cx="19" cy="19" r="3"/><path d="M12 8v3M9.5 13.5L6.5 16.5M14.5 13.5l3 3"/></svg>
  ),
  Eye: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5"><path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z"/><circle cx="12" cy="12" r="3"/></svg>
  ),
  Wrench: ({ size = 24, color = "currentColor" }) => (
    <svg width={size} height={size} viewBox="0 0 24 24" fill="none" stroke={color} strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"><path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z"/></svg>
  ),
};

// ── ROUTING CONTEXT ───────────────────────────────────────────
const RouterCtx = createContext({ page: "hjem", go: () => {} });
function useRouter() { return useContext(RouterCtx); }

// ── PARALLAX HOOK ─────────────────────────────────────────────
function useParallax(speed = 0.3) {
  const ref = useRef(null);
  const [offset, setOffset] = useState(0);
  useEffect(() => {
    const handler = () => {
      if (!ref.current) return;
      const rect = ref.current.getBoundingClientRect();
      const center = rect.top + rect.height / 2 - window.innerHeight / 2;
      setOffset(center * speed);
    };
    window.addEventListener("scroll", handler, { passive: true });
    return () => window.removeEventListener("scroll", handler);
  }, [speed]);
  return { ref, offset };
}

// ── REVEAL ON SCROLL ──────────────────────────────────────────
function Reveal({ children, delay = 0, style = {}, className = "" }) {
  const [vis, setVis] = useState(false);
  const ref = useRef(null);
  useEffect(() => {
    const obs = new IntersectionObserver(([e]) => { if (e.isIntersecting) { setVis(true); obs.disconnect(); } }, { threshold: 0.1 });
    if (ref.current) obs.observe(ref.current);
    return () => obs.disconnect();
  }, []);
  return (
    <div ref={ref} className={className} style={{ ...style, opacity: vis ? 1 : 0, transform: vis ? "translateY(0)" : "translateY(36px)", transition: `opacity .7s cubic-bezier(.16,1,.3,1) ${delay}s, transform .7s cubic-bezier(.16,1,.3,1) ${delay}s` }}>
      {children}
    </div>
  );
}

// ── ANIMATED COUNTER ──────────────────────────────────────────
function Counter({ end, suffix = "" }) {
  const [v, setV] = useState(0);
  const [started, setStarted] = useState(false);
  const ref = useRef(null);
  useEffect(() => {
    const obs = new IntersectionObserver(([e]) => { if (e.isIntersecting) setStarted(true); }, { threshold: 0.3 });
    if (ref.current) obs.observe(ref.current);
    return () => obs.disconnect();
  }, []);
  useEffect(() => {
    if (!started) return;
    let cur = 0;
    const step = Math.max(1, end / 60);
    const t = setInterval(() => { cur += step; if (cur >= end) { setV(end); clearInterval(t); } else setV(Math.floor(cur)); }, 16);
    return () => clearInterval(t);
  }, [started, end]);
  return <span ref={ref}>{v}{suffix}</span>;
}

// ══════════════════════════════════════════════════════════════
// PAGE DATA — Complete knowledge base content
// ══════════════════════════════════════════════════════════════

const PAGES = {
  hjem: { title: "Seobyrå.com", subtitle: "Norges ledende SEO- og AEO-byrå" },
  "teknisk-seo": {
    title: "Teknisk SEO", subtitle: "Grunnmuren for synlighet", icon: "Code",
    hero: "Teknisk SEO handler om å sikre at søkemotorer kan oppdage, crawle, indeksere og forstå nettstedet ditt korrekt. Uten et solid teknisk fundament vil selv det beste innholdet forbli usynlig.",
    sections: [
      { title: "Crawling og indeksering", content: "Googleboten crawler nettet ved å følge lenker fra side til side. For at sidene dine skal indekseres, må de være tilgjengelige via en logisk intern lenkestruktur, ha et oppdatert XML-sitemap, og ikke blokkeres av robots.txt eller noindex-direktiver.\n\nEn vanlig feil er å utilsiktet blokkere viktige sider gjennom feilkonfigurert robots.txt, eller å ha så mange nivåer i nettstedsarkitekturen at Googleboten ikke når de dypeste sidene innenfor sitt crawl-budsjett. Crawl-budsjettet er antall sider Google er villig til å crawle på nettstedet ditt i en gitt periode — for store nettsteder (10 000+ sider) er dette en kritisk faktor." },
      { title: "Core Web Vitals", content: "Core Web Vitals er Googles måleparametere for brukeropplevelse og en bekreftet rangeringsfaktor. De tre målepunktene er:\n\nLargest Contentful Paint (LCP): Hvor raskt det største synlige elementet lastes. Mål: under 2,5 sekunder. Optimaliseres gjennom bildekomprimering, server-side rendering, CDN og eliminering av renderblokkerende ressurser.\n\nInteraction to Next Paint (INP): Erstatter FID fra mars 2024. Måler responshastigheten på brukerinteraksjoner. Mål: under 200ms. Optimaliseres gjennom code splitting, lazy loading og minimering av main thread-arbeid.\n\nCumulative Layout Shift (CLS): Visuell stabilitet — hvor mye elementer flytter seg under lasting. Mål: under 0,1. Fiks ved å definere eksplisitte dimensjoner for bilder/videoer og unngå dynamisk injisert innhold over folden." },
      { title: "Nettstedsarkitektur", content: "En flat, logisk arkitektur sikrer at alle sider er tilgjengelige innen 3 klikk fra forsiden. Siloed architecture (tematisk gruppering) hjelper Google med å forstå tematisk relevans.\n\nBruk breadcrumbs med Schema.org-markup for navigasjon. Interne lenker bør fordele PageRank strategisk — lenk fra sterke sider til sider du ønsker å løfte. Hub-and-spoke-modellen fungerer godt: én pillarside med dyptgående innhold lenker til og fra detaljerte undersider om hvert deltema." },
      { title: "Schema.org og strukturert data", content: "Strukturert data gir søkemotorer maskinlesbar kontekst om innholdet ditt. JSON-LD er det anbefalte formatet. Viktige Schema-typer:\n\nOrganization: Bedriftsinformasjon, logo, kontaktdata.\nFAQPage: Spørsmål og svar som kan vises direkte i søkeresultater.\nHowTo: Trinn-for-trinn-guider med rich snippets.\nArticle: Publiseringsdato, forfatter, hovedbilde.\nBreadcrumbList: Navigasjonssti.\nLocalBusiness: For lokal SEO med adresse, åpningstider, anmeldelser.\n\nStrukturert data er også kritisk for AEO — AI-modeller bruker Schema.org for å tolke og sitere innhold." },
      { title: "Hastighetsoptimalisering", content: "Sidehastighet påvirker både rangering og konvertering. Hvert sekund ekstra lastetid reduserer konverteringen med opptil 7 %. Nøkkeltiltak:\n\nBilder: Bruk WebP/AVIF-format, lazy loading, srcset for responsiv levering.\nJavaScript: Code splitting, tree shaking, defer/async-lasting.\nCSS: Inline kritisk CSS, utsett resten.\nServer: HTTP/2 eller HTTP/3, Brotli-komprimering, edge caching via CDN.\nFonter: font-display: swap, preload kritiske fonter, begrens antall.\n\nBruk PageSpeed Insights, WebPageTest og Chrome DevTools for kontinuerlig overvåkning." },
      { title: "Mobilvennlighet", content: "Google bruker mobile-first indexing — det er mobilversjonen av nettstedet ditt som indekseres og rankes. Responsive design er standard, men sjekk at touchelementer har tilstrekkelig størrelse (minst 48×48px), at innhold ikke er skjult bak click-to-expand på mobil, og at bilder skalerer korrekt.\n\nTest med Googles Mobile-Friendly Test og bruk Chrome DevTools device emulation for å verifisere opplevelsen på ulike skjermstørrelser." },
      { title: "HTTPS og sikkerhet", content: "HTTPS er en bekreftet rangeringsfaktor. Alle sider skal lastes over TLS med gyldig SSL-sertifikat. Sørg for at HTTP-versjoner redirecter med 301 til HTTPS, at mixed content (HTTP-ressurser på HTTPS-sider) elimineres, og at HSTS-headere er konfigurert for å forhindre downgrade-angrep." },
      { title: "Internasjonalisering (hreflang)", content: "For flerspråklige nettsteder brukes hreflang-attributtet til å fortelle Google hvilken språkversjon som skal vises til brukere i ulike regioner. Implementeres i HTML head, HTTP-headers, eller XML-sitemap. Vanlige feil inkluderer manglende x-default, ikke-resiproke hreflang-referanser, og bruk av feil språk-/regionkoder." },
    ]
  },
  "innholdsstrategi": {
    title: "Innholdsstrategi", subtitle: "Innhold som ranker og konverterer", icon: "Pencil",
    hero: "Innholdsstrategi for SEO handler om å skape systematisk, autorativt innhold som dekker hele kundereisen — fra informasjonssøk til kjøpsbeslutning — og som posisjonerer deg som den definitive kilden i din bransje.",
    sections: [
      { title: "Søkeordsanalyse", content: "Søkeordsanalyse er fundamentet for all innholdsstrategi. Prosessen innebærer å identifisere søkeord med relevant volum og oppnåelig konkurranse, og kartlegge søkeintensjonen bak hvert ord.\n\nDe fire søkeintensjonene: Informasjonell (brukeren søker kunnskap: 'hva er SEO'), Navigasjonell (brukeren søker en bestemt side: 'Google Search Console'), Kommersiell (brukeren undersøker alternativer: 'beste SEO-byrå'), og Transaksjonell (brukeren er klar til handling: 'SEO-byrå Oslo pris').\n\nVerktøy: Google Keyword Planner, Ahrefs, SEMrush, Google Search Console, Google Trends. For det norske markedet er det viktig å analysere både bokmål og nynorsk-varianter, samt å forstå at søkevolumene er naturlig lavere enn for engelske søkeord." },
      { title: "Topical authority", content: "Topical authority betyr å bli den mest komplette kilden innenfor et emneområde. I stedet for å skrive enkeltstående artikler, bygger du et tematisk kluster av innhold som dekker hovedtemaet og alle undertemaer.\n\nModellen: Én pillarside (2000-5000 ord) som gir en helhetlig oversikt, omgitt av 10-30 klyngesider som går i dybden på spesifikke undertemaer. Alle sider lenker til og fra pillarsiden. Google belønner denne tilnærmingen fordi den demonstrerer ekspertise, autoritet og troverdighet (E-E-A-T) innenfor temaet." },
      { title: "E-E-A-T: Erfaring, Ekspertise, Autoritet, Troverdighet", content: "E-E-A-T er ikke en direkte rangeringsfaktor, men reflekteres i hundrevis av signaler Google bruker. For YMYL-innhold (Your Money or Your Life — helse, finans, juss) er E-E-A-T spesielt kritisk.\n\nErfaring: Vis at innholdet er basert på førstehåndserfaring. Ekspertise: Kvalifiserte forfattere med synlig forfatterbiografi og lenker til LinkedIn/fagprofiler. Autoritet: Siteres av andre kilder, kvalitetslenker inn. Troverdighet: Oppdatert innhold, korrekt informasjon, transparente kilder, fungerende kontaktinformasjon.\n\nPraktiske tiltak: Forfatterbiografier med ekspertisedokumentasjon, siteringer til primærkilder, oppdateringsdatoer, klare redaksjonelle retningslinjer, og 'Skrevet av / Fagansvarlig'-angivelser." },
      { title: "Innholdsproduksjon", content: "Hver innholdsside bør optimaliseres for én primær søkefrase og 3-5 sekundære fraser. Strukturer med H1 (primær søkefrase), H2-er for delområder, H3-er for detaljer. Bruk av primærordet i tittel, URL, meta description, første avsnitt, og naturlig gjennom teksten.\n\nInnholdslengde: Kvalitet trumfer kvantitet, men for konkurranseutsatte søkeord kreves typisk 1500-3000 ord for å matche konkurrentenes dybde. Bruk featured snippet-optimalisering: svar direkte på spørsmålet i 40-60 ord rett under H2-overskriften." },
      { title: "Innholdsoppdatering og vedlikehold", content: "Google foretrekker oppdatert innhold, spesielt for søk der aktualitet er viktig. Gjør en kvartalsvis innholdsaudit: identifiser sider med synkende trafikk, oppdater fakta og statistikk, konsolider tynt innhold, og redirect eller slett irrelevante sider.\n\nContent decay er reelt — uten vedlikehold mister selv godt innhold rangeringer over tid fordi konkurrenter publiserer nyere, bedre innhold." },
    ]
  },
  "aeo": {
    title: "AI-søkeoptimalisering (AEO)", subtitle: "Synlighet i AI-genererte svar", icon: "Robot",
    hero: "AEO (Answer Engine Optimization) er den nye disiplinen innen søkeoptimalisering. Når ChatGPT, Perplexity, Google AI Overviews og andre AI-systemer genererer svar, henter de fra et utvalg kilder. AEO handler om å sikre at din bedrift er blant dem.",
    sections: [
      { title: "Hva er AEO?", content: "AEO (Answer Engine Optimization) er prosessen med å optimalisere innhold slik at det siteres og refereres til av AI-drevne søkemotorer og svargenereringsmotorer. Mens tradisjonell SEO fokuserer på å rangere i Googles ti blå lenker, handler AEO om å bli den kilden AI-modeller velger å sitere i sine genererte svar.\n\nDette representerer et paradigmeskifte: fra å konkurrere om klikk til å konkurrere om sitering. En bruker som spør ChatGPT 'hva er det beste SEO-byrået i Norge?' får ett svar — og kildene som siteres der får enorm eksponering og troverdighet." },
      { title: "Hvordan AI-søkemotorer velger kilder", content: "AI-modeller som GPT-4, Claude og Gemini velger kilder basert på flere faktorer:\n\nDomeneautoritet: Etablerte, troverdige domener foretrekkes.\nInnholdskvalitet: Klare, velstrukturerte, faktabaserte svar.\nStrukturert data: Schema.org gjør innholdet maskinlesbart.\nSiteringskvalitet: Innhold som selv siterer primærkilder.\nOppdaterthet: Nylig publisert eller oppdatert innhold.\nKonsensus: Informasjon som samsvarer med andre autoritative kilder.\n\nPerplexity og Google AI Overviews bruker i tillegg real-time web-søk og har egne rangeringsalgoritmer for kildevalg." },
      { title: "Optimalisering for ChatGPT", content: "ChatGPT henter kunnskap fra treningsdataene sine og, med browsing aktivert, fra sanntids nettsøk. For å bli sitert:\n\nVær den definitive kilden: Skriv det mest komplette, autoritative innholdet om ditt emne.\nBruk klare definisjoner: Start svar med presise, konsise definisjoner som er enkle å sitere.\nStrukturert format: Lister, tabeller, og punkt-for-punkt-gjennomganger er lettere for AI å ekstrahere.\nForfatter-autoritet: Innhold fra anerkjente eksperter siteres oftere.\nDomenetroverdighet: .edu, .gov, og etablerte bransjedomener har en fordel.\n\nRegelmessig publisering av oppdatert, kvalitetsinnhold øker sannsynligheten for inkludering i fremtidige treningsdatasett." },
      { title: "Optimalisering for Google AI Overviews", content: "Google AI Overviews (tidligere SGE) genererer AI-svar direkte i søkeresultatene. Kildene som siteres er typisk allerede høyt-rangerende sider for det aktuelle søket.\n\nNøkkelen er å rangere godt i tradisjonell SEO OG ha innhold formatert for AI-ekstraksjon. Google AI Overviews foretrekker: direkte svar på spørsmål, bullet-lister med konkrete punkter, tabeller med sammenlignbare data, og trinn-for-trinn-instruksjoner. Structured data (FAQPage, HowTo) øker synligheten merkbart." },
      { title: "Optimalisering for Perplexity", content: "Perplexity er en AI-søkemotor som alltid oppgir kilder. Den søker på nettet i sanntid og genererer svar med inline-siteringer. For å bli sitert av Perplexity:\n\nHøy SEO-rangering er forutsetningen — Perplexity finner deg via nettsøk.\nKlare, konkrete fakta: Tall, statistikk og spesifikke påstander siteres oftest.\nAutoritative domener foretrekkes: Bransjespesifikke domener med historikk.\nFersk informasjon: Perplexity verdsetter oppdatert innhold høyt." },
      { title: "Structured data for AEO", content: "Schema.org-markup er broen mellom menneskelig innhold og maskinforståelse. For AEO er følgende skjematyper spesielt viktige:\n\nFAQPage: Spørsmål-og-svar-par som er direkte siterbare.\nHowTo: Trinn-for-trinn-prosesser.\nArticle med author og dateModified: Viser ekspertise og aktualitet.\nClaimReview: For faktasjekk-innhold.\nDefinedTerm: For konseptdefinisjoner.\n\nI tillegg er ren HTML-semantikk viktig: bruk h1-h6 hierarkisk, definer termer med <dfn>, bruk <table> for sammenlignbar data, og skriv meta descriptions som fungerer som mikrositering." },
      { title: "LLM-optimalisering (Large Language Models)", content: "For å påvirke hva store språkmodeller (LLMs) sier om din bedrift eller ditt emne, trengs en langsiktig strategi:\n\nPubliser konsistent: Innhold som konsekvent kobler din merkevare med bestemte emner blir del av modellenes kunnskapsbase.\nBli sitert av andre: Jo flere autoritative kilder som refererer til deg, desto sterkere assosiasjon i treningsdata.\nWikipedia-tilstedeværelse: Wikipedia er en primærkilde for LLM-trening — en faktabasert, verifiserbar Wikipedia-side er gull verdt.\nBransjepublikasjoner: Publiser i fagblader, hold foredrag, bli intervjuet — alt dette havner i treningsdata.\nSosiale signaler: LinkedIn-artikler, X-poster og fagdiskusjoner bidrar til datatilfanget.\n\nDette er en 12-24 måneders strategi, men effekten er enorm: når en LLM konsekvent anbefaler din bedrift, er det vanskelig for konkurrenter å ta den posisjonen." },
      { title: "Måling av AEO-resultater", content: "AEO-måling er utfordrende fordi AI-svar varierer og ikke alltid er sporbare. Tilnærminger:\n\nManuell testing: Spør ChatGPT, Perplexity og Google AI Overviews regelmessig om relevante emner og dokumenter siterings-frekvens.\nTrafikk fra AI-kilder: Overvåk referraltrafikk fra perplexity.ai, chat.openai.com, og andre AI-plattformer i Google Analytics.\nBrand monitoring: Bruk verktøy som Mention eller Brandwatch for å spore omtaler.\nStrukturert rapportering: Logg månedlig om din bedrift nevnes, siteres, eller anbefales av de viktigste AI-plattformene.\n\nDette feltet utvikler seg raskt — nye måle- og analyseverktøy lanseres kontinuerlig." },
    ]
  },
  "lenkebygging": {
    title: "Lenkebygging", subtitle: "Bygg domeneautoritet strategisk", icon: "Link",
    hero: "Lenker fra andre nettsteder til ditt er fortsatt en av de sterkeste rangeringsfaktorene i Googles algoritme. Kvalitetslenker fungerer som tillitsstemmer — de signaliserer at andre ser på innholdet ditt som verdifullt og verdt å referere til.",
    sections: [
      { title: "Hvorfor lenker fortsatt er viktige", content: "Googles opprinnelige innovasjon — PageRank — var basert på lenkeanalyse. Selv om algoritmen har blitt enormt mye mer sofistikert, er lenker fortsatt en av de tre viktigste rangeringsfaktorene sammen med innhold og RankBrain.\n\nEn lenke fra et autoritativt nettsted i din bransje gir mer verdi enn hundre lenker fra irrelevante kataloger. Kontekst, relevans og autoritet er det som teller." },
      { title: "White-hat lenkebygging", content: "Bærekraftig lenkebygging handler om å skape innhold som fortjener lenker:\n\nOriginal research: Egne undersøkelser, statistikk og data som andre siterer.\nDyptgående guider: Den definitive ressursen om et emne.\nVerktøy og kalkulatorer: Gratis verktøy som løser problemer.\nDigital PR: Nyhetsverdig innhold som journalister dekker.\nGjesteinnlegg: Publiser fagartikler på bransjerelevante nettsteder.\nBroken link building: Finn døde lenker hos andre og tilby ditt innhold som erstatning.\nRessurssider: Bli inkludert i bransjens ressurslister og guider." },
      { title: "Lenker å unngå", content: "Google identifiserer og straffer manipulative lenkemetoder:\n\nKjøpte lenker: Direkte kjøp av lenker bryter Googles retningslinjer.\nPBN-er (Private Blog Networks): Nettverk av sider bygget kun for lenkebygging.\nAutomatiserte lenker: Programmatisk genererte lenker i kommentarfelt, forum, etc.\nLenkefarmer: Nettverk der alle lenker til alle uten redaksjonell verdi.\nIrrelevante kataloger: Masse-innmelding i hundrevis av irrelevante kataloger.\n\nStraffen kan være algoritmisk (gradvis synlighetstap) eller manuell (nedrangering med varsel i Search Console). Recovery fra en manuell straff kan ta 6-12 måneder." },
      { title: "Intern lenkebygging", content: "Interne lenker er undervurdert. En strategisk intern lenkestruktur fordeler PageRank til sidene som trenger det, hjelper Google med å forstå innholdshierarki, og leder brukere gjennom konverteringstrakten.\n\nBruk deskriptive ankertekster (ikke 'klikk her'). Lenk fra høyautoritets-sider til nye eller svake sider du vil løfte. Opprett tematiske klynger med pillarside og klyngesider som lenker til hverandre." },
    ]
  },
  "lokal-seo": {
    title: "Lokal SEO", subtitle: "Dominer i ditt nærområde", icon: "MapPin",
    hero: "Lokal SEO handler om å bli synlig for kunder som søker i ditt geografiske område. 46 % av alle Google-søk har lokal intensjon, og 76 % av de som søker lokalt besøker en bedrift innen 24 timer.",
    sections: [
      { title: "Google Business Profile", content: "Google Business Profile (tidligere Google My Business) er det viktigste verktøyet for lokal SEO. En komplett, optimalisert profil øker sjansen for å vises i Local Pack (de tre resultatene med kart øverst i søket).\n\nOptimalisering: Velg riktige kategorier (primær + sekundær). Skriv en detaljert bedriftsbeskrivelse med relevante søkeord. Last opp minst 10 kvalitetsbilder. Publiser Google Posts ukentlig. Svar på alle anmeldelser — positive og negative. Hold åpningstider og kontaktinfo 100 % oppdatert.\n\nNAP-konsistens (Name, Address, Phone) på tvers av alle plattformer er kritisk. Bruk eksakt samme format overalt." },
      { title: "Lokale landingssider", content: "For bedrifter med flere lokasjoner, lag unike landingssider for hvert sted. Hver side skal ha unikt innhold, lokale referanser, stedsspesifikke bilder, og LocalBusiness Schema-markup med adresse, koordinater og åpningstider.\n\nInnholdet skal ikke bare bytte ut bynavnet — det skal være genuint lokalt med referanser til nærområdet, lokale kunder, og stedsspesifikk informasjon." },
      { title: "Anmeldelser og omdømmehåndtering", content: "Google-anmeldelser er en topp 3 rangeringsfaktor for Local Pack. Strategier: be fornøyde kunder om anmeldelse med direktelenke. Svar på alle anmeldelser innen 24 timer. Håndter negative anmeldelser profesjonelt og konstruktivt.\n\nMål: minst 4,0 i gjennomsnittscore, og en jevn strøm av nye anmeldelser (Google verdsetter ferske anmeldelser høyere). Ikke tilby insentiver for anmeldelser — det bryter Googles retningslinjer." },
    ]
  },
  "on-page-seo": {
    title: "On-page SEO", subtitle: "Optimaliser hver enkelt side", icon: "File",
    hero: "On-page SEO er kunsten å optimalisere individuelle sider for søkemotorer. Det dekker alt fra titler og meta descriptions til innholdsstruktur, intern lenking, bildeoptimalisering og brukeropplevelse.",
    sections: [
      { title: "Tittel-tag og meta description", content: "Tittel-taggen er det viktigste on-page-elementet. Inkluder primærordet tidlig, hold lengden under 60 tegn, og skriv for klikk — ikke bare for Google.\n\nMeta description påvirker ikke rangering direkte, men påvirker klikkrate (CTR) som er et indirekte signal. Hold den under 155 tegn, inkluder en call-to-action, og bruk primærordet naturlig. Google erstatter ofte meta description med egen tekst fra innholdet — men en god meta description øker sjansen for at din tekst brukes." },
      { title: "Overskriftshierarki", content: "Bruk H1 for sidens hovedoverskrift (inneholder primærordet). H2-er for hovedseksjoner. H3-er for underseksjoner. Ikke hopp over nivåer. Overskriftene skal skape et logisk hierarki som Google kan bruke til å forstå innholdsstrukturen.\n\nTips: Skriv H2-er som spørsmål brukere stiller — dette øker sjansen for featured snippets." },
      { title: "URL-struktur", content: "Korte, beskrivende URL-er med søkeord er foretrukket. Bruk bindestrek mellom ord. Unngå tall, datoer og parametre i URL-er.\n\nEksempel: /teknisk-seo er bedre enn /artikler/2024/01/alt-du-trenger-a-vite-om-teknisk-seo-for-nybegynnere\n\nNår en URL er publisert og indeksert, unngå å endre den med mindre det er strengt nødvendig — og bruk alltid 301-redirect." },
      { title: "Bildeoptimalisering", content: "Bilder skal ha beskrivende filnavn (teknisk-seo-sjekkliste.webp, ikke IMG_4523.jpg), alt-tekst som beskriver bildet med relevante søkeord, og være komprimert til minst mulig filstørrelse uten synlig kvalitetstap.\n\nBruk WebP eller AVIF-format. Implementer lazy loading. Definer width og height for å unngå CLS. Vurder srcset for responsiv bildelasting." },
    ]
  },
  "sokemotorer": {
    title: "Søkemotorer", subtitle: "Forstå landskapet", icon: "Globe",
    hero: "En søkemotor er et system som indekserer innhold på nettet og returnerer relevante resultater basert på brukerens søk. Google dominerer med over 90 % markedsandel i Norge, men AI-drevne alternativer vokser raskt.",
    sections: [
      { title: "Google", content: "Google prosesserer over 8,5 milliarder søk per dag globalt. I Norge er markedsandelen over 93 %. Algoritmen bruker hundrevis av rangeringsfaktorer, men de viktigste er innholdskvalitet, lenker og brukeropplevelse.\n\nGoogle oppdaterer algoritmen kontinuerlig med core updates (3-4 per år), spam updates, og spesifikke oppdateringer som Helpful Content Update og Reviews Update. Å forstå hva disse oppdateringene belønner og straffer er essensielt for SEO-arbeid." },
      { title: "Google AI Overviews", content: "Lansert i 2024, AI Overviews er Googles AI-genererte svarblokk som vises over tradisjonelle søkeresultater for mange spørsmål. Den trekker fra flere kilder og presenterer et sammenfattet svar.\n\nFor SEO betyr dette at posisjon 1 ikke lenger garanterer synlighet — brukeren kan få svaret uten å klikke. AEO-strategi er nødvendig for å sikre at din side er blant kildene som siteres." },
      { title: "Bing og Microsoft Copilot", content: "Bing har ca. 3-4 % markedsandel i Norge, men er viktig av to grunner: det driver Microsoft Copilot (AI-assistenten integrert i Windows, Office og Edge), og Bing-indeksen brukes av flere AI-søkemotorer.\n\nBing Webmaster Tools er undervurdert — det gir innsikt som Google Search Console ikke tilbyr, og optimalisering for Bing krever mange av de samme tiltakene som for Google." },
      { title: "Perplexity", content: "Perplexity er en AI-native søkemotor som kombinerer nettsøk med AI-genererte svar og alltid oppgir kilder med inline-siteringer. Den vokser raskt blant kunnskapssøkere og profesjonelle.\n\nFor AEO er Perplexity en nøkkelplattform fordi den er transparent om kilder — du kan se nøyaktig når innholdet ditt siteres." },
      { title: "ChatGPT Search", content: "OpenAIs ChatGPT har fått integrert nettsøk som konkurrerer direkte med Google. Med over 200 millioner ukentlige brukere er ChatGPT nå en betydelig søkeplattform, spesielt for research-tunge søk.\n\nChatGPT Search bruker Bing-indeksen for nettresultater, noe som gjør Bing-optimalisering enda mer relevant." },
    ]
  },
  "konvertering": {
    title: "Konverteringsoptimalisering", subtitle: "Fra trafikk til kunder", icon: "Chart",
    hero: "Organisk trafikk uten konvertering er bare en vanitetsmetrikk. Konverteringsoptimalisering (CRO) handler om å designe brukerreisen slik at besøkende fra søk faktisk gjennomfører den handlingen du ønsker — enten det er en henvendelse, et kjøp, eller en påmelding.",
    sections: [
      { title: "Landingsside-optimalisering", content: "En landingsside fra organisk søk må oppfylle søkeintensjonen umiddelbart. Brukeren har stilt et spørsmål — svaret ditt bør være synlig over folden.\n\nSjekkliste: Klar overskrift som matcher søkeordet. Verdiforslag synlig innen 3 sekunder. Tydelig CTA (call-to-action) over folden. Tillitssignaler: anmeldelser, kundelogoer, sertifiseringer. Rask lasting (under 2,5 sekunder LCP). Mobiloptimalisert med store touchelementer." },
      { title: "CTA-strategi", content: "Bruk primær og sekundær CTA: primær for handlingsklare (Bestill gratis analyse), sekundær for research-fasen (Les mer om våre tjenester). Plasser CTA-er strategisk: over folden, etter nøkkelargumenter, og i sticky elementer." },
      { title: "A/B-testing", content: "Test systematisk med verktøy som Google Optimize (nå integrert i GA4), VWO eller Optimizely. Test én variabel om gangen: overskrifter, CTA-tekst, layout, farger. La tester kjøre til statistisk signifikans (minimum 95 % konfidensintervall)." },
    ]
  },
  "analyse": {
    title: "SEO-analyse og verktøy", subtitle: "Datadrevet optimalisering", icon: "Gauge",
    hero: "Effektiv SEO krever kontinuerlig måling og analyse. Med de rette verktøyene og KPI-ene kan du identifisere muligheter, spore fremgang, og justere strategi basert på data — ikke gjetning.",
    sections: [
      { title: "Google Search Console", content: "Google Search Console (GSC) er det viktigste gratisverktøyet for SEO. Det viser hvilke søkeord som genererer visninger og klikk, indekseringstatus, Core Web Vitals, og eventuelle problemer Google har funnet.\n\nNøkkelrapporter: Ytelsesrapporten (søkeord, sider, CTR, posisjon), Indeksering (dekningsrapport, sitemap-status), Erfaring (Core Web Vitals, mobilbrukbarhet), og Forbedringer (strukturert data, breadcrumbs)." },
      { title: "Google Analytics 4", content: "GA4 erstatter Universal Analytics og gir innsikt i brukeratferd etter at de ankommer nettstedet. For SEO er de viktigste rapportene: Trafikkanskaffelse (organisk vs. andre kanaler), Engasjement (tid på side, bounce rate, sider per sesjon), og Konverteringer.\n\nSett opp hendelsesbaserte konverteringsmål for å spore verdien av organisk trafikk direkte." },
      { title: "Tredjepartsverktøy", content: "Ahrefs: Best for lenkeanalyse, konkurrentovervåkning, og innholdsgap-analyse. SEMrush: Bred plattform med søkeordsovervåking, site audit, og konkurranseanalyse. Screaming Frog: Teknisk SEO-crawler for å identifisere feil. Google PageSpeed Insights: Core Web Vitals-målinger. Schema Markup Validator: Valider strukturert data." },
      { title: "KPI-er for SEO", content: "Organisk trafikk: Totalt antall besøk fra organisk søk. Søkeordrangeringer: Posisjoner for prioriterte søkeord. Synlighetsindeks: Samlet synlighetsverdi (fra Ahrefs/SEMrush/Sistrix). Organisk CTR: Klikkrate fra søkeresultater. Konverteringer fra organisk: Handlinger gjennomført av organiske besøkende. Sideindeksering: Andel av sider som er indeksert. Core Web Vitals: LCP, INP, CLS-verdier. Lenkestatistikk: Antall og kvalitet på inngående lenker." },
    ]
  },
  "ordliste": {
    title: "SEO-ordliste", subtitle: "Komplett fagordliste A-Å", icon: "File",
    hero: "En komplett ordliste over de viktigste begrepene innen SEO, AEO og digital synlighet. Fra algoritmer til zero-click-søk.",
    sections: [
      { title: "A", content: "AEO (Answer Engine Optimization): Optimalisering for AI-drevne svargenereringsmotorer. Alt-tekst: Beskrivende tekst for bilder, brukt av søkemotorer og skjermlesere. Algoritme: Settet med regler søkemotorer bruker for å rangere sider. Ankertekst: Den klikkbare teksten i en lenke. Autoritet: Et nettsteds troverdighet og styrke i søkemotorenes øyne." },
      { title: "B-C", content: "Backlink: En lenke fra et annet nettsted til ditt. Black hat SEO: Manipulative teknikker som bryter søkemotorenes retningslinjer. Bounce rate: Andelen besøkende som forlater siden uten interaksjon. Canonical URL: Den foretrukne versjonen av en side med duplikatinnhold. Core Web Vitals: Googles måleparametere for brukeropplevelse (LCP, INP, CLS). Crawling: Prosessen der søkemotorer skanner nettsider. CTR (Click-Through Rate): Klikkrate fra søkeresultater." },
      { title: "D-F", content: "Domain Authority: Moz-metrikk for domenetstyrke (0-100). Domain Rating: Ahrefs-metrikk for domenetstyrke (0-100). Dwell time: Tid brukt på en side etter klikk fra søkeresultater. E-E-A-T: Experience, Expertise, Authoritativeness, Trustworthiness. Featured snippet: Fremhevet svar øverst i Googles søkeresultater. Freshness: Hvor nylig innhold er publisert eller oppdatert." },
      { title: "G-I", content: "Google AI Overviews: AI-generert svarblokk i Google-søk. Google Business Profile: Bedriftsprofil i Google for lokal synlighet. GSC (Google Search Console): Gratisverktøy for SEO-overvåking. Hreflang: HTML-attributt for å angi språk/region-versjoner. Indeksering: Prosessen der søkemotorer lagrer og organiserer nettsider. Intern lenke: Lenke mellom sider på samme nettsted." },
      { title: "J-N", content: "JSON-LD: Format for strukturert data anbefalt av Google. Keyword cannibalization: Når flere sider konkurrerer om samme søkeord. Knowledge Graph: Googles kunnskapsdatabase for entiteter. LLM (Large Language Model): Store språkmodeller som GPT-4, Claude, Gemini. Local Pack: De tre lokale resultatene med kart i Google. Meta description: HTML-tag som beskriver sidens innhold. Mobile-first indexing: Google indekserer mobilversjonen primært. NAP: Name, Address, Phone — konsistens på tvers av nett." },
      { title: "O-S", content: "Off-page SEO: Optimalisering utenfor nettstedet (lenker, omtaler). On-page SEO: Optimalisering av individuelle sider. Organisk trafikk: Besøk fra ubetalte søkeresultater. PageRank: Googles opprinnelige algoritme for lenkeanalyse. Pillarside: Hovedside i et innholdskluster. Robots.txt: Fil som instruerer søkemotorer om hva de kan crawle. Schema.org: Vokabular for strukturert data. SERP: Search Engine Results Page. Sitemap: XML-fil som lister alle sider for søkemotorer." },
      { title: "T-Å", content: "Teknisk SEO: Optimalisering av nettstedets tekniske infrastruktur. Topical authority: Autoritet innenfor et spesifikt emneområde. URL: Uniform Resource Locator — nettadresse. UX (User Experience): Brukeropplevelse. White hat SEO: Etiske SEO-teknikker som følger retningslinjene. YMYL: Your Money or Your Life — innhold som påvirker helse, økonomi eller sikkerhet. Zero-click search: Søk der brukeren får svar uten å klikke inn på et nettsted." },
    ]
  },
  "nettverk": {
    title: "Vårt kunnskapsnettverk", subtitle: "Norges mest omfattende SEO-økosystem", icon: "Network",
    hero: "Vi eier og drifter et nettverk av autoritative kunnskapsportaler som sammen utgjør Norges mest komplette ressurs innen SEO, AI-søk og digital synlighet. Hvert domene er spesialisert innenfor sitt emneområde og bygger topical authority gjennom dyptgående, ekspertskrevet innhold.",
    sections: [
      { title: "seoai.no — AI-drevet SEO", content: "Norges ledende kunnskapsportal for skjæringspunktet mellom kunstig intelligens og søkemotoroptimalisering. Dekker AI-verktøy for SEO, maskinlæring i søkealgoritmer, automatisert innholdsoptimalisering, og hvordan AI transformerer hele SEO-bransjen." },
      { title: "ai-seo.no — AI & SEO", content: "Praktiske guider og strategier for å bruke AI i SEO-arbeid. Fra prompt engineering for innholdsproduksjon til AI-assistert søkeordsanalyse, konkurrentovervåkning og teknisk optimalisering." },
      { title: "organisksynlighet.no — Organisk synlighet", content: "Helhetlig ressurs om hvordan bedrifter oppnår og måler organisk synlighet. Dekker synlighetsindekser, SEO-strategi, innholdsmarkedsføring, og langsiktig merkevarebygging gjennom organiske kanaler." },
      { title: "organisksøk.no — Organisk søk", content: "Dyptgående innhold om organiske søkeresultater — hvordan de fungerer, hva som påvirker rangering, og strategier for å dominere organisk søk i det norske markedet." },
      { title: "organisktrafikk.no — Organisk trafikk", content: "Alt om å generere, analysere og øke organisk trafikk. Fra Google Analytics-oppsett til trafikkvekststrategier, segmentering og konvertering av organiske besøkende." },
      { title: "ai-søk.no — AI-søk", content: "Dedikert til den nye æraen av AI-drevne søkemotorer. Dekker ChatGPT Search, Perplexity, Google AI Overviews, Claude, og kommende AI-søketeknologier — og hva dette betyr for bedrifter." },
      { title: "søkemotor.com — Søkemotorer", content: "Kunnskapsbasen om søkemotorer — fra Googles historie og algoritme til alternative søkemotorer, søkemotortrender, og teknologien bak moderne informasjonsgjenfinning." },
      { title: "søkeoptimalisering.no — Søkeoptimalisering", content: "Norges mest komplette guide til søkeoptimalisering. Den ultimate ressursen for alle som vil forstå og mestre SEO — fra grunnleggende konsepter til avanserte strategier." },
    ]
  },
  "om-oss": {
    title: "Om Seobyrå.com", subtitle: "Norges nye SEO-kraftsenter", icon: "Shield",
    hero: "Seobyrå.com er Norges nye SEO- og AEO-byrå med en unik posisjon: vi kombinerer tradisjonell søkemotoroptimalisering med banebrytende AI-søkeoptimalisering, støttet av Norges mest omfattende nettverk av autoritative kunnskapsportaler.",
    sections: [
      { title: "Vår tilnærming", content: "Vi tror på datadrevet SEO med full transparens. Ingen magiske formler eller hemmelig saus — bare metodisk arbeid basert på teknisk fundament, kvalitetsinnhold, og strategisk autoritetsbygging.\n\nVår unike fordel er at vi eier og drifter et nettverk av kunnskapsportaler som gir oss førstehånds innsikt i hva som faktisk fungerer i norske søkeresultater. Vi tester og verifiserer strategier på egne domener før vi implementerer dem for kunder." },
      { title: "Tjenesteoversikt", content: "Teknisk SEO: Crawlability, indeksering, hastighet, Core Web Vitals, Schema.org.\nInnholdsstrategi: Søkeordsanalyse, topical authority, innholdsproduksjon, E-E-A-T.\nAI-søkeoptimalisering: Optimalisering for ChatGPT, Perplexity, Google AI Overviews.\nLenkebygging: Strategisk autoritetsbygging gjennom kvalitetslenker.\nLokal SEO: Google Business Profile, lokale landingssider, anmeldelser.\nKonverteringsoptimalisering: Landingssideoptimalisering, CTA-strategi, A/B-testing." },
      { title: "En del av IT-FIRMA", content: "Seobyrå.com er en del av IT-FIRMA, et norsk teknologiselskap med bred kompetanse innen digital utvikling, hosting og markedsføring. Denne tilhørigheten gir oss tilgang til teknisk infrastruktur og utviklingsressurser som setter oss i stand til å levere helhetlige løsninger." },
    ]
  },
  "kontakt": {
    title: "Kontakt oss", subtitle: "Gratis synlighetsanalyse", icon: "Target",
    hero: "Ta kontakt for en uforpliktende samtale om din digitale synlighet. Vi analyserer nettstedet ditt, kartlegger konkurrentene, og gir deg en konkret handlingsplan — helt gratis.",
    sections: []
  },
};

const NAV_ITEMS = [
  { id: "hjem", label: "Hjem" },
  { id: "tjenester", label: "Tjenester", children: [
    { id: "teknisk-seo", label: "Teknisk SEO" },
    { id: "innholdsstrategi", label: "Innholdsstrategi" },
    { id: "aeo", label: "AI-søkeoptimalisering" },
    { id: "lenkebygging", label: "Lenkebygging" },
    { id: "lokal-seo", label: "Lokal SEO" },
    { id: "on-page-seo", label: "On-page SEO" },
    { id: "konvertering", label: "Konvertering" },
  ]},
  { id: "kunnskap", label: "Kunnskap", children: [
    { id: "sokemotorer", label: "Søkemotorer" },
    { id: "analyse", label: "Analyse & verktøy" },
    { id: "ordliste", label: "SEO-ordliste" },
  ]},
  { id: "nettverk", label: "Nettverk" },
  { id: "om-oss", label: "Om oss" },
  { id: "kontakt", label: "Kontakt" },
];

// ══════════════════════════════════════════════════════════════
// COMPONENTS
// ══════════════════════════════════════════════════════════════

function Navbar() {
  const { page, go } = useRouter();
  const [scrolled, setScrolled] = useState(false);
  const [mobileOpen, setMobileOpen] = useState(false);
  const [hoveredMenu, setHoveredMenu] = useState(null);

  useEffect(() => {
    const h = () => setScrolled(window.scrollY > 40);
    window.addEventListener("scroll", h, { passive: true });
    return () => window.removeEventListener("scroll", h);
  }, []);

  return (
    <nav style={{
      position: "fixed", top: 0, left: 0, right: 0, zIndex: 1000,
      background: scrolled ? "rgba(8,8,10,0.92)" : "transparent",
      backdropFilter: scrolled ? "blur(24px) saturate(1.2)" : "none",
      borderBottom: scrolled ? "1px solid rgba(255,255,255,0.04)" : "1px solid transparent",
      transition: "all .4s ease",
    }}>
      <div style={{ maxWidth: 1260, margin: "0 auto", display: "flex", justifyContent: "space-between", alignItems: "center", height: 72, padding: "0 clamp(20px, 4vw, 48px)" }}>
        <button onClick={() => go("hjem")} style={{ background: "none", border: "none", cursor: "pointer", display: "flex", alignItems: "center", gap: 10 }}>
          <svg width="28" height="28" viewBox="0 0 28 28" fill="none">
            <rect width="28" height="28" rx="6" fill="#c8ff00"/>
            <path d="M8 18.5c0-2 1.2-3.8 3-4.5 1-.4 2.2-.4 3 0M17 9.5a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0zM21 14l-3-3v2h-3v2h3v2l3-3z" stroke="#08080a" strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"/>
          </svg>
          <span style={{ fontSize: 17, fontWeight: 700, color: "#e8e6e1", letterSpacing: "-0.03em", fontFamily: "var(--font-display)" }}>SEOBYRÅ<span style={{ fontWeight: 400, color: "rgba(255,255,255,0.3)", fontSize: 13 }}>.com</span></span>
        </button>

        <div style={{ display: "flex", alignItems: "center", gap: 4 }}>
          {NAV_ITEMS.map(item => (
            <div key={item.id} style={{ position: "relative" }}
              onMouseEnter={() => item.children && setHoveredMenu(item.id)}
              onMouseLeave={() => setHoveredMenu(null)}>
              <button onClick={() => !item.children && go(item.id)} style={{
                background: "none", border: "none", color: page === item.id ? "#c8ff00" : "rgba(255,255,255,0.55)",
                fontSize: 13.5, fontWeight: 500, padding: "8px 14px", cursor: "pointer", fontFamily: "inherit",
                display: "flex", alignItems: "center", gap: 4, transition: "color .2s",
                letterSpacing: "0.01em",
              }}>
                {item.label}
                {item.children && <Icon.ChevronDown size={12} />}
              </button>
              {item.children && hoveredMenu === item.id && (
                <div style={{
                  position: "absolute", top: "100%", left: 0, minWidth: 220,
                  background: "rgba(16,16,20,0.97)", border: "1px solid rgba(255,255,255,0.06)",
                  borderRadius: 8, padding: "8px 0", backdropFilter: "blur(20px)",
                  boxShadow: "0 16px 48px rgba(0,0,0,0.5)",
                }}>
                  {item.children.map(child => (
                    <button key={child.id} onClick={() => { go(child.id); setHoveredMenu(null); }} style={{
                      display: "flex", alignItems: "center", gap: 10, width: "100%", padding: "10px 18px",
                      background: page === child.id ? "rgba(200,255,0,0.06)" : "none",
                      border: "none", color: page === child.id ? "#c8ff00" : "rgba(255,255,255,0.6)",
                      fontSize: 13.5, cursor: "pointer", fontFamily: "inherit", textAlign: "left", transition: "all .15s",
                    }}
                    onMouseEnter={e => { e.currentTarget.style.background = "rgba(255,255,255,0.04)"; e.currentTarget.style.color = "#e8e6e1"; }}
                    onMouseLeave={e => { e.currentTarget.style.background = page === child.id ? "rgba(200,255,0,0.06)" : "none"; e.currentTarget.style.color = page === child.id ? "#c8ff00" : "rgba(255,255,255,0.6)"; }}>
                      {Icon[PAGES[child.id]?.icon] && (() => { const I = Icon[PAGES[child.id].icon]; return <I size={16} />; })()}
                      {child.label}
                    </button>
                  ))}
                </div>
              )}
            </div>
          ))}
          <button onClick={() => go("kontakt")} style={{
            marginLeft: 8, padding: "9px 22px", background: "#c8ff00", color: "#08080a",
            border: "none", fontSize: 13, fontWeight: 600, cursor: "pointer", fontFamily: "inherit",
            letterSpacing: "0.03em", transition: "all .2s",
          }}
          onMouseEnter={e => { e.currentTarget.style.background = "#dfff4f"; e.currentTarget.style.transform = "translateY(-1px)"; }}
          onMouseLeave={e => { e.currentTarget.style.background = "#c8ff00"; e.currentTarget.style.transform = ""; }}>
            Gratis analyse
          </button>
        </div>
      </div>
    </nav>
  );
}

function HomePage() {
  const { go } = useRouter();
  const parallax1 = useParallax(0.15);
  const parallax2 = useParallax(-0.1);

  const services = [
    { id: "teknisk-seo", icon: "Code", title: "Teknisk SEO", desc: "Crawling, indeksering, Core Web Vitals, Schema.org og nettstedsarkitektur" },
    { id: "innholdsstrategi", icon: "Pencil", title: "Innholdsstrategi", desc: "Søkeordsanalyse, topical authority, E-E-A-T og innholdsproduksjon" },
    { id: "aeo", icon: "Robot", title: "AI-søkeoptimalisering", desc: "Synlighet i ChatGPT, Perplexity og Google AI Overviews" },
    { id: "lenkebygging", icon: "Link", title: "Lenkebygging", desc: "Strategisk autoritetsbygging gjennom kvalitetslenker" },
    { id: "lokal-seo", icon: "MapPin", title: "Lokal SEO", desc: "Google Business Profile og dominans i lokale søk" },
    { id: "konvertering", icon: "Chart", title: "Konvertering", desc: "Fra organisk trafikk til henvendelser og salg" },
  ];

  return (
    <>
      {/* HERO */}
      <header style={{ minHeight: "100vh", display: "flex", alignItems: "center", position: "relative", overflow: "hidden", padding: "120px clamp(20px, 4vw, 48px) 80px" }}>
        <div style={{ position: "absolute", top: "5%", right: "-5%", width: "50vw", height: "50vw", background: "radial-gradient(circle, rgba(200,255,0,0.035) 0%, transparent 65%)", pointerEvents: "none" }} ref={parallax1.ref} />
        <div style={{ position: "absolute", inset: 0, background: "linear-gradient(180deg, transparent 60%, rgba(8,8,10,1))", pointerEvents: "none" }} />
        {/* Grid lines decoration */}
        <div style={{ position: "absolute", top: 0, left: "10%", width: 1, height: "100%", background: "rgba(255,255,255,0.02)", pointerEvents: "none" }} />
        <div style={{ position: "absolute", top: 0, left: "30%", width: 1, height: "100%", background: "rgba(255,255,255,0.02)", pointerEvents: "none" }} />
        <div style={{ position: "absolute", top: 0, right: "20%", width: 1, height: "100%", background: "rgba(255,255,255,0.02)", pointerEvents: "none" }} />

        <div style={{ maxWidth: 1260, margin: "0 auto", width: "100%", position: "relative", zIndex: 1 }}>
          <Reveal>
            <div style={{ display: "inline-flex", alignItems: "center", gap: 8, padding: "7px 18px", border: "1px solid rgba(200,255,0,0.2)", marginBottom: 40, fontSize: 12.5, fontWeight: 500, color: "#c8ff00", letterSpacing: "0.04em" }}>
              <span style={{ width: 6, height: 6, background: "#c8ff00", borderRadius: "50%", animation: "pulse 2.5s infinite" }} />
              SEO + AEO — tradisjonell og AI-søkeoptimalisering
            </div>
          </Reveal>
          <Reveal delay={0.08}>
            <h1 style={{ fontFamily: "var(--font-display)", fontSize: "clamp(2.8rem, 6.5vw, 5.8rem)", fontWeight: 300, lineHeight: 1.04, letterSpacing: "-0.035em", maxWidth: 850 }}>
              Bli den kilden<br />
              <span style={{ fontWeight: 600 }}>søkemotorer</span> og<br />
              <em style={{ fontStyle: "italic", color: "#c8ff00", fontWeight: 300 }}>AI siterer</em>
            </h1>
          </Reveal>
          <Reveal delay={0.16}>
            <p style={{ fontSize: "clamp(15px, 1.6vw, 18px)", lineHeight: 1.7, color: "rgba(255,255,255,0.45)", maxWidth: 520, marginTop: 28 }}>
              Vi kombinerer søkemotoroptimalisering med AI-søkeoptimalisering for norske bedrifter. Resultatet: synlighet i Google, ChatGPT, Perplexity og AI Overviews.
            </p>
          </Reveal>
          <Reveal delay={0.24}>
            <div style={{ display: "flex", gap: 14, marginTop: 44, flexWrap: "wrap" }}>
              <button onClick={() => go("kontakt")} className="btn-primary" style={{ display: "inline-flex", alignItems: "center", gap: 10, padding: "15px 32px", background: "#c8ff00", color: "#08080a", border: "none", fontSize: 14, fontWeight: 600, cursor: "pointer", fontFamily: "inherit", letterSpacing: "0.03em", transition: "all .25s" }}
                onMouseEnter={e => { e.currentTarget.style.background = "#dfff4f"; e.currentTarget.style.transform = "translateY(-2px)"; e.currentTarget.style.boxShadow = "0 8px 32px rgba(200,255,0,0.2)"; }}
                onMouseLeave={e => { e.currentTarget.style.background = "#c8ff00"; e.currentTarget.style.transform = ""; e.currentTarget.style.boxShadow = ""; }}>
                Bestill gratis synlighetsanalyse <Icon.Arrow size={16} />
              </button>
              <button onClick={() => go("teknisk-seo")} style={{ display: "inline-flex", alignItems: "center", gap: 10, padding: "15px 32px", background: "transparent", color: "#e8e6e1", border: "1px solid rgba(255,255,255,0.12)", fontSize: 14, fontWeight: 500, cursor: "pointer", fontFamily: "inherit", transition: "all .25s" }}
                onMouseEnter={e => { e.currentTarget.style.borderColor = "#c8ff00"; e.currentTarget.style.color = "#c8ff00"; }}
                onMouseLeave={e => { e.currentTarget.style.borderColor = "rgba(255,255,255,0.12)"; e.currentTarget.style.color = "#e8e6e1"; }}>
                Utforsk kunnskapsbasen
              </button>
            </div>
          </Reveal>
          <Reveal delay={0.35}>
            <div style={{ display: "grid", gridTemplateColumns: "repeat(4, 1fr)", gap: 0, marginTop: 72, borderTop: "1px solid rgba(255,255,255,0.06)", paddingTop: 36 }}>
              {[["150+", "søkeord på side 1"], ["47", "aktive kunder"], ["340%", "snitt trafikkvekst"], ["8+", "års erfaring"]].map(([val, label], i) => (
                <div key={label} style={{ borderLeft: i > 0 ? "1px solid rgba(255,255,255,0.06)" : "none", paddingLeft: i > 0 ? 24 : 0 }}>
                  <div style={{ fontSize: "clamp(26px, 3.5vw, 40px)", fontWeight: 700, letterSpacing: "-0.03em", fontFamily: "var(--font-display)" }}>{val}</div>
                  <div style={{ fontSize: 12.5, color: "rgba(255,255,255,0.3)", marginTop: 4, letterSpacing: "0.02em" }}>{label}</div>
                </div>
              ))}
            </div>
          </Reveal>
        </div>
      </header>

      {/* SERVICES GRID */}
      <section style={{ padding: "100px clamp(20px, 4vw, 48px)", position: "relative" }}>
        <div style={{ maxWidth: 1260, margin: "0 auto" }}>
          <Reveal>
            <div style={{ marginBottom: 56 }}>
              <span style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.14em", textTransform: "uppercase", color: "#c8ff00" }}>Tjenester</span>
              <h2 style={{ fontFamily: "var(--font-display)", fontSize: "clamp(1.8rem, 3.5vw, 2.8rem)", fontWeight: 300, lineHeight: 1.15, letterSpacing: "-0.025em", marginTop: 12 }}>
                Helhetlig søkeoptimalisering<br />for den <em style={{ fontStyle: "italic", fontWeight: 600 }}>nye æraen</em>
              </h2>
            </div>
          </Reveal>
          <div style={{ display: "grid", gridTemplateColumns: "repeat(3, 1fr)", gap: 1 }}>
            {services.map((s, i) => {
              const I = Icon[s.icon];
              return (
                <Reveal key={s.id} delay={i * 0.06}>
                  <button onClick={() => go(s.id)} style={{
                    width: "100%", padding: "40px 32px", background: "rgba(255,255,255,0.012)",
                    border: "1px solid rgba(255,255,255,0.04)", cursor: "pointer", textAlign: "left",
                    fontFamily: "inherit", color: "#e8e6e1", transition: "all .35s ease", position: "relative",
                    overflow: "hidden", minHeight: 200,
                  }}
                  onMouseEnter={e => { e.currentTarget.style.borderColor = "rgba(200,255,0,0.25)"; e.currentTarget.style.background = "rgba(200,255,0,0.02)"; e.currentTarget.style.transform = "translateY(-3px)"; }}
                  onMouseLeave={e => { e.currentTarget.style.borderColor = "rgba(255,255,255,0.04)"; e.currentTarget.style.background = "rgba(255,255,255,0.012)"; e.currentTarget.style.transform = ""; }}>
                    <div style={{ marginBottom: 20, color: "#c8ff00" }}><I size={28} /></div>
                    <h3 style={{ fontSize: 19, fontWeight: 600, marginBottom: 10, letterSpacing: "-0.01em" }}>{s.title}</h3>
                    <p style={{ fontSize: 14, lineHeight: 1.65, color: "rgba(255,255,255,0.4)" }}>{s.desc}</p>
                    <div style={{ display: "flex", alignItems: "center", gap: 6, marginTop: 20, fontSize: 13, fontWeight: 500, color: "#c8ff00" }}>
                      Les mer <Icon.Arrow size={14} color="#c8ff00" />
                    </div>
                  </button>
                </Reveal>
              );
            })}
          </div>
        </div>
      </section>

      {/* AEO HIGHLIGHT */}
      <section style={{ padding: "100px clamp(20px, 4vw, 48px)", borderTop: "1px solid rgba(200,255,0,0.06)", borderBottom: "1px solid rgba(200,255,0,0.06)", background: "linear-gradient(180deg, rgba(200,255,0,0.015) 0%, transparent 100%)", position: "relative" }} ref={parallax2.ref}>
        <div style={{ maxWidth: 1260, margin: "0 auto", display: "grid", gridTemplateColumns: "1.1fr 1fr", gap: 72, alignItems: "center" }}>
          <Reveal>
            <div>
              <span style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.14em", textTransform: "uppercase", color: "#c8ff00" }}>Ny disiplin</span>
              <h2 style={{ fontFamily: "var(--font-display)", fontSize: "clamp(1.8rem, 3.5vw, 2.6rem)", fontWeight: 300, lineHeight: 1.2, letterSpacing: "-0.025em", marginTop: 12, marginBottom: 20 }}>
                AI-søk endrer alt.<br />Er din bedrift <em style={{ fontStyle: "italic", fontWeight: 600, color: "#c8ff00" }}>forberedt?</em>
              </h2>
              <p style={{ fontSize: 15, lineHeight: 1.8, color: "rgba(255,255,255,0.45)", marginBottom: 14 }}>
                ChatGPT, Perplexity og Google AI Overviews genererer nå svar med kilder. I stedet for ti blå lenker får brukeren ett svar og tre referanser.
              </p>
              <p style={{ fontSize: 15, lineHeight: 1.8, color: "rgba(255,255,255,0.45)", marginBottom: 28 }}>
                Vi sørger for at din bedrift er den referansen. Gjennom strukturert data, autoritative kunnskapsportaler og strategisk AEO-arbeid bygger vi tilstedeværelsen din der det teller.
              </p>
              <button onClick={() => go("aeo")} style={{ display: "inline-flex", alignItems: "center", gap: 8, padding: "13px 28px", background: "#c8ff00", color: "#08080a", border: "none", fontSize: 13.5, fontWeight: 600, cursor: "pointer", fontFamily: "inherit", transition: "all .2s" }}
                onMouseEnter={e => { e.currentTarget.style.background = "#dfff4f"; }}
                onMouseLeave={e => { e.currentTarget.style.background = "#c8ff00"; }}>
                Lær om AEO <Icon.Arrow size={14} />
              </button>
            </div>
          </Reveal>
          <Reveal delay={0.12}>
            <div style={{ background: "rgba(255,255,255,0.02)", border: "1px solid rgba(255,255,255,0.06)", borderRadius: 10, padding: 32 }}>
              <div style={{ fontSize: 11.5, fontWeight: 500, color: "rgba(255,255,255,0.25)", letterSpacing: "0.06em", textTransform: "uppercase", marginBottom: 20, display: "flex", alignItems: "center", gap: 8 }}>
                <Icon.Robot size={14} color="rgba(255,255,255,0.3)" /> AI-generert svar
              </div>
              <div style={{ background: "rgba(200,255,0,0.04)", borderRadius: 8, padding: 20, border: "1px solid rgba(200,255,0,0.08)", marginBottom: 20 }}>
                <p style={{ fontSize: 14, lineHeight: 1.7, color: "rgba(255,255,255,0.65)" }}>
                  For å forbedre organisk synlighet bør bedrifter fokusere på teknisk SEO, innholdskvalitet, strukturert data og AI-søkeoptimalisering (AEO)...
                </p>
              </div>
              <div style={{ fontSize: 11, color: "rgba(255,255,255,0.25)", marginBottom: 10, letterSpacing: "0.04em" }}>Kilder</div>
              {[{ name: "seobyrå.com", highlight: true }, { name: "kilde2.no" }, { name: "kilde3.no" }].map(s => (
                <div key={s.name} style={{ display: "flex", alignItems: "center", gap: 10, padding: "9px 14px", marginBottom: 6, borderRadius: 6, background: s.highlight ? "rgba(200,255,0,0.06)" : "rgba(255,255,255,0.02)", border: s.highlight ? "1px solid rgba(200,255,0,0.12)" : "1px solid transparent" }}>
                  <div style={{ width: 6, height: 6, borderRadius: "50%", background: s.highlight ? "#c8ff00" : "rgba(255,255,255,0.12)" }} />
                  <span style={{ fontSize: 13, fontWeight: s.highlight ? 600 : 400, color: s.highlight ? "#c8ff00" : "rgba(255,255,255,0.3)" }}>{s.name}</span>
                  {s.highlight && <span style={{ fontSize: 11, color: "rgba(255,255,255,0.25)", marginLeft: "auto" }}>Din bedrift</span>}
                </div>
              ))}
            </div>
          </Reveal>
        </div>
      </section>

      {/* RESULTS */}
      <section style={{ padding: "100px clamp(20px, 4vw, 48px)" }}>
        <div style={{ maxWidth: 1260, margin: "0 auto" }}>
          <Reveal>
            <span style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.14em", textTransform: "uppercase", color: "#c8ff00" }}>Resultater</span>
            <h2 style={{ fontFamily: "var(--font-display)", fontSize: "clamp(1.8rem, 3.5vw, 2.8rem)", fontWeight: 300, lineHeight: 1.15, letterSpacing: "-0.025em", marginTop: 12, marginBottom: 56 }}>
              Dokumenterte <em style={{ fontStyle: "italic", fontWeight: 600 }}>resultater</em>
            </h2>
          </Reveal>
          <div style={{ display: "grid", gridTemplateColumns: "repeat(4, 1fr)", gap: 14 }}>
            {[
              { industry: "Eiendom", metric: "+340%", label: "Organisk trafikk", period: "12 mnd" },
              { industry: "Finans", metric: "+520%", label: "Organiske leads", period: "8 mnd" },
              { industry: "Helse", metric: "+180%", label: "Synlighetsindeks", period: "6 mnd" },
              { industry: "E-handel", metric: "+290%", label: "Organisk omsetning", period: "10 mnd" },
            ].map((c, i) => (
              <Reveal key={i} delay={i * 0.08}>
                <div style={{ background: "rgba(255,255,255,0.015)", border: "1px solid rgba(255,255,255,0.04)", padding: 32, position: "relative", overflow: "hidden", transition: "all .3s" }}
                  onMouseEnter={e => { e.currentTarget.style.borderColor = "rgba(200,255,0,0.2)"; e.currentTarget.style.transform = "translateY(-2px)"; }}
                  onMouseLeave={e => { e.currentTarget.style.borderColor = "rgba(255,255,255,0.04)"; e.currentTarget.style.transform = ""; }}>
                  <div style={{ position: "absolute", top: 0, left: 0, right: 0, height: 2, background: `linear-gradient(90deg, #c8ff00 ${30 + i * 18}%, transparent)` }} />
                  <span style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.25)", letterSpacing: "0.08em", textTransform: "uppercase" }}>{c.industry}</span>
                  <div style={{ fontSize: 44, fontWeight: 700, color: "#c8ff00", letterSpacing: "-0.04em", lineHeight: 1, marginTop: 16, fontFamily: "var(--font-display)" }}>{c.metric}</div>
                  <div style={{ fontSize: 14, fontWeight: 500, marginTop: 8 }}>{c.label}</div>
                  <div style={{ fontSize: 12, color: "rgba(255,255,255,0.25)", marginTop: 2 }}>{c.period}</div>
                </div>
              </Reveal>
            ))}
          </div>
        </div>
      </section>

      {/* CTA */}
      <section style={{ padding: "80px clamp(20px, 4vw, 48px)", borderTop: "1px solid rgba(200,255,0,0.06)" }}>
        <div style={{ maxWidth: 700, margin: "0 auto", textAlign: "center" }}>
          <Reveal>
            <h2 style={{ fontFamily: "var(--font-display)", fontSize: "clamp(1.8rem, 3.5vw, 2.8rem)", fontWeight: 300, lineHeight: 1.15, letterSpacing: "-0.025em", marginBottom: 16 }}>
              Klar for å bli <em style={{ fontStyle: "italic", fontWeight: 600, color: "#c8ff00" }}>synlig?</em>
            </h2>
            <p style={{ fontSize: 15, color: "rgba(255,255,255,0.45)", lineHeight: 1.7, marginBottom: 36 }}>
              Vi analyserer nettstedet ditt, kartlegger konkurrentene, og gir deg en konkret handlingsplan. Helt gratis og uforpliktende.
            </p>
            <button onClick={() => go("kontakt")} style={{ display: "inline-flex", alignItems: "center", gap: 10, padding: "16px 40px", background: "#c8ff00", color: "#08080a", border: "none", fontSize: 15, fontWeight: 600, cursor: "pointer", fontFamily: "inherit", transition: "all .25s" }}
              onMouseEnter={e => { e.currentTarget.style.background = "#dfff4f"; e.currentTarget.style.transform = "translateY(-2px)"; e.currentTarget.style.boxShadow = "0 10px 40px rgba(200,255,0,0.2)"; }}
              onMouseLeave={e => { e.currentTarget.style.background = "#c8ff00"; e.currentTarget.style.transform = ""; e.currentTarget.style.boxShadow = ""; }}>
              Bestill gratis synlighetsanalyse <Icon.Arrow size={16} />
            </button>
          </Reveal>
        </div>
      </section>
    </>
  );
}

function ContentPage({ pageId }) {
  const { go } = useRouter();
  const page = PAGES[pageId];
  if (!page || !page.sections) return null;
  const I = Icon[page.icon];
  const parallax = useParallax(0.12);

  // Find related pages
  const allServicePages = ["teknisk-seo", "innholdsstrategi", "aeo", "lenkebygging", "lokal-seo", "on-page-seo", "konvertering", "sokemotorer", "analyse", "ordliste", "nettverk", "om-oss"];
  const related = allServicePages.filter(p => p !== pageId).slice(0, 3);

  return (
    <>
      {/* Page hero */}
      <header style={{ paddingTop: 140, paddingBottom: 60, padding: "140px clamp(20px, 4vw, 48px) 60px", position: "relative", overflow: "hidden" }}>
        <div style={{ position: "absolute", top: 0, right: "-10%", width: "40vw", height: "40vw", background: "radial-gradient(circle, rgba(200,255,0,0.025) 0%, transparent 65%)", pointerEvents: "none" }} ref={parallax.ref} />
        <div style={{ maxWidth: 820, margin: "0 auto", position: "relative", zIndex: 1 }}>
          <Reveal>
            <button onClick={() => go("hjem")} style={{ display: "flex", alignItems: "center", gap: 6, background: "none", border: "none", color: "rgba(255,255,255,0.35)", fontSize: 13, cursor: "pointer", fontFamily: "inherit", marginBottom: 32, transition: "color .2s" }}
              onMouseEnter={e => e.currentTarget.style.color = "#c8ff00"}
              onMouseLeave={e => e.currentTarget.style.color = "rgba(255,255,255,0.35)"}>
              <span style={{ transform: "rotate(180deg)", display: "inline-flex" }}><Icon.Arrow size={14} /></span> Tilbake til forsiden
            </button>
          </Reveal>
          <Reveal delay={0.05}>
            <div style={{ display: "flex", alignItems: "center", gap: 14, marginBottom: 20 }}>
              {I && <div style={{ color: "#c8ff00" }}><I size={32} /></div>}
              <span style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.12em", textTransform: "uppercase", color: "#c8ff00" }}>{page.subtitle}</span>
            </div>
          </Reveal>
          <Reveal delay={0.1}>
            <h1 style={{ fontFamily: "var(--font-display)", fontSize: "clamp(2.2rem, 5vw, 3.6rem)", fontWeight: 300, lineHeight: 1.1, letterSpacing: "-0.03em" }}>{page.title}</h1>
          </Reveal>
          <Reveal delay={0.16}>
            <p style={{ fontSize: 16.5, lineHeight: 1.75, color: "rgba(255,255,255,0.5)", marginTop: 24, maxWidth: 700 }}>{page.hero}</p>
          </Reveal>
        </div>
      </header>

      {/* Table of contents */}
      {page.sections.length > 3 && (
        <div style={{ padding: "0 clamp(20px, 4vw, 48px)", marginBottom: 48 }}>
          <div style={{ maxWidth: 820, margin: "0 auto", padding: "24px 28px", background: "rgba(255,255,255,0.015)", border: "1px solid rgba(255,255,255,0.04)", borderRadius: 4 }}>
            <div style={{ fontSize: 12, fontWeight: 600, color: "rgba(255,255,255,0.3)", letterSpacing: "0.08em", textTransform: "uppercase", marginBottom: 14 }}>Innhold</div>
            <div style={{ display: "grid", gridTemplateColumns: page.sections.length > 6 ? "1fr 1fr" : "1fr", gap: "6px 24px" }}>
              {page.sections.map((s, i) => (
                <span key={i} style={{ fontSize: 14, color: "rgba(255,255,255,0.5)", lineHeight: 1.6 }}>
                  <span style={{ color: "rgba(200,255,0,0.4)", marginRight: 8, fontSize: 12, fontWeight: 600 }}>{String(i + 1).padStart(2, "0")}</span>
                  {s.title}
                </span>
              ))}
            </div>
          </div>
        </div>
      )}

      {/* Content sections */}
      <div style={{ padding: "0 clamp(20px, 4vw, 48px) 80px" }}>
        <div style={{ maxWidth: 820, margin: "0 auto" }}>
          {page.sections.map((s, i) => (
            <Reveal key={i} delay={0.04}>
              <article style={{ marginBottom: 56, paddingBottom: 56, borderBottom: i < page.sections.length - 1 ? "1px solid rgba(255,255,255,0.04)" : "none" }}>
                <div style={{ display: "flex", alignItems: "baseline", gap: 14, marginBottom: 16 }}>
                  <span style={{ fontSize: 11, fontWeight: 700, color: "rgba(200,255,0,0.3)", letterSpacing: "0.06em" }}>{String(i + 1).padStart(2, "0")}</span>
                  <h2 style={{ fontFamily: "var(--font-display)", fontSize: "clamp(1.3rem, 2.5vw, 1.7rem)", fontWeight: 500, letterSpacing: "-0.015em" }}>{s.title}</h2>
                </div>
                {s.content.split("\n\n").map((para, j) => (
                  <p key={j} style={{ fontSize: 15.5, lineHeight: 1.85, color: "rgba(255,255,255,0.55)", marginBottom: 16 }}>{para}</p>
                ))}
              </article>
            </Reveal>
          ))}
        </div>
      </div>

      {/* Related pages */}
      <div style={{ padding: "60px clamp(20px, 4vw, 48px) 80px", borderTop: "1px solid rgba(255,255,255,0.04)" }}>
        <div style={{ maxWidth: 1260, margin: "0 auto" }}>
          <Reveal>
            <h3 style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.12em", textTransform: "uppercase", color: "#c8ff00", marginBottom: 28 }}>Les videre</h3>
          </Reveal>
          <div style={{ display: "grid", gridTemplateColumns: "repeat(3, 1fr)", gap: 14 }}>
            {related.map((rid, i) => {
              const rp = PAGES[rid];
              if (!rp) return null;
              const RI = Icon[rp.icon];
              return (
                <Reveal key={rid} delay={i * 0.06}>
                  <button onClick={() => go(rid)} style={{
                    width: "100%", padding: "28px 24px", background: "rgba(255,255,255,0.012)",
                    border: "1px solid rgba(255,255,255,0.04)", cursor: "pointer", textAlign: "left",
                    fontFamily: "inherit", color: "#e8e6e1", transition: "all .3s",
                  }}
                  onMouseEnter={e => { e.currentTarget.style.borderColor = "rgba(200,255,0,0.2)"; e.currentTarget.style.transform = "translateY(-2px)"; }}
                  onMouseLeave={e => { e.currentTarget.style.borderColor = "rgba(255,255,255,0.04)"; e.currentTarget.style.transform = ""; }}>
                    <div style={{ color: "#c8ff00", marginBottom: 12 }}>{RI && <RI size={22} />}</div>
                    <h4 style={{ fontSize: 16, fontWeight: 600, marginBottom: 6 }}>{rp.title}</h4>
                    <p style={{ fontSize: 13, color: "rgba(255,255,255,0.35)", lineHeight: 1.5 }}>{rp.subtitle}</p>
                  </button>
                </Reveal>
              );
            })}
          </div>
        </div>
      </div>
    </>
  );
}

function ContactPage() {
  const [form, setForm] = useState({ name: "", email: "", url: "", msg: "" });
  return (
    <div style={{ paddingTop: 140, padding: "140px clamp(20px, 4vw, 48px) 80px" }}>
      <div style={{ maxWidth: 1100, margin: "0 auto", display: "grid", gridTemplateColumns: "1fr 1fr", gap: 72 }}>
        <Reveal>
          <div>
            <span style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.14em", textTransform: "uppercase", color: "#c8ff00" }}>Kom i gang</span>
            <h1 style={{ fontFamily: "var(--font-display)", fontSize: "clamp(2rem, 4vw, 3rem)", fontWeight: 300, lineHeight: 1.15, letterSpacing: "-0.025em", marginTop: 12, marginBottom: 20 }}>
              Gratis <em style={{ fontStyle: "italic", fontWeight: 600, color: "#c8ff00" }}>synlighetsanalyse</em>
            </h1>
            <p style={{ fontSize: 15.5, lineHeight: 1.75, color: "rgba(255,255,255,0.45)", marginBottom: 36 }}>
              Vi kartlegger din nåværende synlighet, analyserer konkurrentene, og gir deg en konkret handlingsplan. Helt gratis og uforpliktende.
            </p>
            {["Teknisk SEO-sjekk av nettstedet ditt", "Konkurranseanalyse for dine viktigste søkeord", "Konkrete anbefalinger for forbedring", "Estimat på potensiell trafikkvekst", "AEO-analyse: synlighet i AI-søk"].map(item => (
              <div key={item} style={{ display: "flex", alignItems: "center", gap: 12, marginBottom: 14 }}>
                <div style={{ width: 20, height: 20, borderRadius: 3, background: "rgba(200,255,0,0.08)", display: "flex", alignItems: "center", justifyContent: "center", flexShrink: 0 }}>
                  <svg width="12" height="12" viewBox="0 0 12 12" fill="none" stroke="#c8ff00" strokeWidth="2" strokeLinecap="round"><path d="M2 6l3 3 5-5"/></svg>
                </div>
                <span style={{ fontSize: 14.5, color: "rgba(255,255,255,0.55)" }}>{item}</span>
              </div>
            ))}
          </div>
        </Reveal>
        <Reveal delay={0.1}>
          <div style={{ background: "rgba(255,255,255,0.015)", border: "1px solid rgba(255,255,255,0.06)", borderRadius: 4, padding: "36px 32px" }}>
            {[
              { label: "Navn", key: "name", placeholder: "Ditt navn", type: "text" },
              { label: "E-post", key: "email", placeholder: "din@epost.no", type: "email" },
              { label: "Nettside", key: "url", placeholder: "https://dinnettside.no", type: "text" },
            ].map(f => (
              <div key={f.key} style={{ marginBottom: 28 }}>
                <label style={{ fontSize: 11.5, fontWeight: 600, color: "rgba(255,255,255,0.25)", letterSpacing: "0.08em", textTransform: "uppercase", display: "block", marginBottom: 8 }}>{f.label}</label>
                <input type={f.type} placeholder={f.placeholder} value={form[f.key]} onChange={e => setForm({ ...form, [f.key]: e.target.value })} style={{ width: "100%", padding: "12px 0", fontSize: 15, fontFamily: "inherit", background: "transparent", border: "none", borderBottom: "1px solid rgba(255,255,255,0.1)", color: "#e8e6e1", outline: "none" }} onFocus={e => e.target.style.borderBottomColor = "#c8ff00"} onBlur={e => e.target.style.borderBottomColor = "rgba(255,255,255,0.1)"} />
              </div>
            ))}
            <div style={{ marginBottom: 28 }}>
              <label style={{ fontSize: 11.5, fontWeight: 600, color: "rgba(255,255,255,0.25)", letterSpacing: "0.08em", textTransform: "uppercase", display: "block", marginBottom: 8 }}>Melding</label>
              <textarea placeholder="Fortell oss kort om din bedrift og hva du ønsker å oppnå..." value={form.msg} onChange={e => setForm({ ...form, msg: e.target.value })} style={{ width: "100%", padding: "12px 0", fontSize: 15, fontFamily: "inherit", background: "transparent", border: "none", borderBottom: "1px solid rgba(255,255,255,0.1)", color: "#e8e6e1", outline: "none", resize: "none", minHeight: 80 }} onFocus={e => e.target.style.borderBottomColor = "#c8ff00"} onBlur={e => e.target.style.borderBottomColor = "rgba(255,255,255,0.1)"} />
            </div>
            <button style={{ width: "100%", padding: "16px 32px", background: "#c8ff00", color: "#08080a", border: "none", fontSize: 14.5, fontWeight: 600, cursor: "pointer", fontFamily: "inherit", transition: "all .2s" }}
              onMouseEnter={e => { e.currentTarget.style.background = "#dfff4f"; }}
              onMouseLeave={e => { e.currentTarget.style.background = "#c8ff00"; }}>
              Send forespørsel
            </button>
            <p style={{ fontSize: 12.5, color: "rgba(255,255,255,0.2)", textAlign: "center", marginTop: 16, lineHeight: 1.5 }}>
              Vi svarer innen 24 timer. Ingen bindingstid.
            </p>
          </div>
        </Reveal>
      </div>
    </div>
  );
}

function Footer() {
  const { go } = useRouter();
  const links = [
    { label: "Tjenester", items: [
      { id: "teknisk-seo", label: "Teknisk SEO" }, { id: "innholdsstrategi", label: "Innholdsstrategi" },
      { id: "aeo", label: "AI-søkeoptimalisering" }, { id: "lenkebygging", label: "Lenkebygging" },
      { id: "lokal-seo", label: "Lokal SEO" }, { id: "konvertering", label: "Konvertering" },
    ]},
    { label: "Kunnskap", items: [
      { id: "sokemotorer", label: "Søkemotorer" }, { id: "on-page-seo", label: "On-page SEO" },
      { id: "analyse", label: "Analyse & verktøy" }, { id: "ordliste", label: "SEO-ordliste" },
    ]},
    { label: "Nettverk", items: [
      { label: "seoai.no" }, { label: "ai-seo.no" }, { label: "organisksynlighet.no" },
      { label: "organisksøk.no" }, { label: "søkeoptimalisering.no" },
    ]},
    { label: "Selskap", items: [
      { id: "om-oss", label: "Om oss" }, { id: "kontakt", label: "Kontakt" }, { id: "nettverk", label: "Vårt nettverk" },
    ]},
  ];

  return (
    <footer style={{ borderTop: "1px solid rgba(255,255,255,0.04)", padding: "56px clamp(20px, 4vw, 48px) 36px" }}>
      <div style={{ maxWidth: 1260, margin: "0 auto" }}>
        <div style={{ display: "grid", gridTemplateColumns: "1.2fr 1fr 1fr 1fr 1fr", gap: 32, marginBottom: 48 }}>
          <div>
            <div style={{ display: "flex", alignItems: "center", gap: 8, marginBottom: 14 }}>
              <svg width="24" height="24" viewBox="0 0 28 28" fill="none"><rect width="28" height="28" rx="6" fill="#c8ff00"/><path d="M8 18.5c0-2 1.2-3.8 3-4.5 1-.4 2.2-.4 3 0M17 9.5a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0zM21 14l-3-3v2h-3v2h3v2l3-3z" stroke="#08080a" strokeWidth="1.5" strokeLinecap="round" strokeLinejoin="round"/></svg>
              <span style={{ fontSize: 16, fontWeight: 700, fontFamily: "var(--font-display)" }}>SEOBYRÅ<span style={{ fontWeight: 400, color: "rgba(255,255,255,0.3)", fontSize: 12 }}>.com</span></span>
            </div>
            <p style={{ fontSize: 13.5, color: "rgba(255,255,255,0.3)", lineHeight: 1.65, maxWidth: 260 }}>
              Norges SEO- og AEO-byrå. Vi gjør bedrifter synlige i søkemotorer og AI-genererte svar.
            </p>
          </div>
          {links.map(group => (
            <div key={group.label}>
              <div style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.2)", letterSpacing: "0.08em", textTransform: "uppercase", marginBottom: 16 }}>{group.label}</div>
              {group.items.map(item => (
                <div key={item.label}>
                  {item.id ? (
                    <button onClick={() => go(item.id)} style={{ display: "block", background: "none", border: "none", fontSize: 13.5, color: "rgba(255,255,255,0.4)", cursor: "pointer", fontFamily: "inherit", padding: "3px 0", transition: "color .2s" }}
                      onMouseEnter={e => e.currentTarget.style.color = "#c8ff00"}
                      onMouseLeave={e => e.currentTarget.style.color = "rgba(255,255,255,0.4)"}>
                      {item.label}
                    </button>
                  ) : (
                    <span style={{ display: "block", fontSize: 13.5, color: "rgba(255,255,255,0.4)", padding: "3px 0" }}>{item.label}</span>
                  )}
                </div>
              ))}
            </div>
          ))}
        </div>
        <div style={{ borderTop: "1px solid rgba(255,255,255,0.04)", paddingTop: 20, display: "flex", justifyContent: "space-between", flexWrap: "wrap", gap: 12 }}>
          <span style={{ fontSize: 12.5, color: "rgba(255,255,255,0.18)" }}>© 2026 Seobyrå.com — Alle rettigheter forbeholdt.</span>
          <span style={{ fontSize: 12.5, color: "rgba(255,255,255,0.14)" }}>En del av <span style={{ color: "rgba(255,255,255,0.3)", fontWeight: 600 }}>IT-FIRMA</span></span>
        </div>
      </div>
    </footer>
  );
}

// ══════════════════════════════════════════════════════════════
// APP SHELL
// ══════════════════════════════════════════════════════════════

export default function App() {
  const [page, setPage] = useState("hjem");

  const go = useCallback((id) => {
    setPage(id);
    window.scrollTo({ top: 0, behavior: "smooth" });
  }, []);

  const renderPage = () => {
    if (page === "hjem") return <HomePage />;
    if (page === "kontakt") return <ContactPage />;
    if (PAGES[page]) return <ContentPage pageId={page} />;
    return <HomePage />;
  };

  return (
    <RouterCtx.Provider value={{ page, go }}>
      <div style={{ fontFamily: "var(--font-body)", color: "#e8e6e1", background: "#08080a", minHeight: "100vh", overflowX: "hidden" }}>
        <style>{`
          @import url('https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=DM+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400&display=swap');
          :root {
            --font-display: 'Instrument Serif', Georgia, 'Times New Roman', serif;
            --font-body: 'DM Sans', -apple-system, BlinkMacSystemFont, sans-serif;
            --accent: #c8ff00;
            --bg: #08080a;
            --text: #e8e6e1;
          }
          * { margin: 0; padding: 0; box-sizing: border-box; }
          html { scroll-behavior: smooth; -webkit-font-smoothing: antialiased; }
          ::selection { background: #c8ff00; color: #08080a; }
          @keyframes pulse { 0%, 100% { opacity: 1; } 50% { opacity: 0.4; } }
          body { background: #08080a; }
        `}</style>

        <Navbar />
        <main>{renderPage()}</main>
        <Footer />
      </div>
    </RouterCtx.Provider>
  );
}
