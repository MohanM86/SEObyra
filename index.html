import { useState, useEffect, useRef } from "react";

// Animated number counter
function Counter({ end, suffix = "", prefix = "", duration = 2000 }) {
  const [count, setCount] = useState(0);
  const [started, setStarted] = useState(false);
  const ref = useRef(null);
  useEffect(() => {
    const obs = new IntersectionObserver(([e]) => { if (e.isIntersecting) setStarted(true); }, { threshold: 0.3 });
    if (ref.current) obs.observe(ref.current);
    return () => obs.disconnect();
  }, []);
  useEffect(() => {
    if (!started) return;
    let start = 0;
    const step = end / (duration / 16);
    const timer = setInterval(() => {
      start += step;
      if (start >= end) { setCount(end); clearInterval(timer); }
      else setCount(Math.floor(start));
    }, 16);
    return () => clearInterval(timer);
  }, [started, end, duration]);
  return <span ref={ref}>{prefix}{count.toLocaleString("nb-NO")}{suffix}</span>;
}

// Reveal on scroll
function Reveal({ children, delay = 0, style = {} }) {
  const [visible, setVisible] = useState(false);
  const ref = useRef(null);
  useEffect(() => {
    const obs = new IntersectionObserver(([e]) => { if (e.isIntersecting) setVisible(true); }, { threshold: 0.15 });
    if (ref.current) obs.observe(ref.current);
    return () => obs.disconnect();
  }, []);
  return (
    <div ref={ref} style={{
      ...style,
      opacity: visible ? 1 : 0,
      transform: visible ? "translateY(0)" : "translateY(32px)",
      transition: `opacity 0.7s ease ${delay}s, transform 0.7s ease ${delay}s`,
    }}>{children}</div>
  );
}

const SERVICES = [
  { num: "01", title: "Teknisk SEO", desc: "Vi avdekker og fikser de tekniske hindringene som holder nettstedet ditt tilbake. Crawlability, indeksering, Core Web Vitals, strukturert data og nettstedsarkitektur — alt som gjør at Google forstår og prioriterer sidene dine.", icon: "⚙️" },
  { num: "02", title: "Innholdsstrategi", desc: "Søkeordsanalyse, innholdsplanlegging og produksjon av autoritativt innhold som ranker. Vi bygger topical authority gjennom systematisk dekning av hele emneområdet ditt.", icon: "✍️" },
  { num: "03", title: "AI-søkeoptimalisering", desc: "Optimaliser for ChatGPT, Perplexity og Google AI Overviews. Vi sørger for at din bedrift blir sitert som kilde når AI-søkemotorer genererer svar — den nye frontlinjen i synlighet.", icon: "🤖" },
  { num: "04", title: "Lenkebygging", desc: "Strategisk oppbygging av domenets autoritet gjennom kvalitetslenker fra relevante, norske nettsteder. Ingen kjøpte PBN-lenker — kun ekte, redaksjonelle plasseringer.", icon: "🔗" },
  { num: "05", title: "Lokal SEO", desc: "Dominér i lokale søk og Google Maps. Google Business-profil, lokale landingssider, stedsspesifikt innhold og konsistent NAP-data på tvers av alle plattformer.", icon: "📍" },
  { num: "06", title: "Konverteringsoptimalisering", desc: "Trafikk alene er ikke nok. Vi optimaliserer brukerreisen fra søkeresultat til konvertering — slik at organisk trafikk faktisk blir til henvendelser og salg.", icon: "📈" },
];

const CASES = [
  { industry: "Eiendom", metric: "+340%", label: "Organisk trafikk", period: "12 måneder", detail: "Fra side 4 til topp 3 på 15 konkurranseutsatte søkeord" },
  { industry: "Finans", metric: "+520%", label: "Organiske leads", period: "8 måneder", detail: "Dominerer nå 'forbrukslån', 'billån' og relaterte søk" },
  { industry: "Helse", metric: "+180%", label: "Synlighetsindeks", period: "6 måneder", detail: "Bygget topical authority som Norges fremste kilde" },
  { industry: "E-handel", metric: "+290%", label: "Organisk omsetning", period: "10 måneder", detail: "Fra 12 % til 38 % av total omsetning via organisk søk" },
];

const NETWORK = [
  { domain: "seoai.no", label: "AI-drevet SEO", desc: "Kunstig intelligens møter søkeoptimalisering" },
  { domain: "ai-seo.no", label: "AI & SEO", desc: "Fremtiden for søkemotoroptimalisering" },
  { domain: "organisksynlighet.no", label: "Organisk synlighet", desc: "Bli synlig uten å betale for hvert klikk" },
  { domain: "organisksøk.no", label: "Organisk søk", desc: "Alt om organiske søkeresultater" },
  { domain: "organisktrafikk.no", label: "Organisk trafikk", desc: "Forstå og øk din organiske trafikk" },
  { domain: "ai-søk.no", label: "AI-søk", desc: "Den nye æraen av AI-drevne søkemotorer" },
  { domain: "søkemotor.com", label: "Søkemotorer", desc: "Kunnskapsbasen om søkemotorer" },
  { domain: "søkeoptimalisering.no", label: "Søkeoptimalisering", desc: "Norges mest komplette SEO-guide" },
];

const FAQ_ITEMS = [
  { q: "Hva koster SEO?", a: "Våre engasjementer starter på 15 000 kr/mnd for lokal SEO og skalerer til 40 000+ kr/mnd for nasjonal SEO i konkurranseutsatte bransjer. Prisen avhenger av konkurransenivå, antall søkeord og omfanget av teknisk arbeid som trengs. Vi gir alltid et konkret tilbud etter en gratis synlighetsanalyse." },
  { q: "Hvor lang tid tar det å se resultater?", a: "SEO er en langsiktig investering. Typisk ser vi første forbedringer etter 2–3 måneder, tydelige resultater etter 4–6 måneder, og full effekt etter 8–12 måneder. Lokale søk gir ofte raskere resultater enn nasjonale. Vi setter alltid klare milepæler og rapporterer månedlig." },
  { q: "Hva er AI-søkeoptimalisering (AEO)?", a: "AEO (Answer Engine Optimization) handler om å optimalisere innhold slik at det siteres av AI-søkemotorer som ChatGPT, Perplexity og Google AI Overviews. Dette krever strukturert data, autoritative kilder, og innhold formatert for maskinlesing — en ny disiplin vi har spesialisert oss på." },
  { q: "Hvordan skiller dere dere fra andre SEO-byråer?", a: "Vi kombinerer tradisjonell SEO med AI-søkeoptimalisering — noe svært få norske byråer gjør. I tillegg eier og opererer vi et nettverk av autoritative kunnskapsportaler som gir oss unik innsikt i hva som faktisk ranker i norske søkeresultater." },
  { q: "Tilbyr dere SEO for små bedrifter?", a: "Ja. Vår lokale SEO-pakke er skreddersydd for små og mellomstore bedrifter som vil dominere i sitt nærområde. Google Business-optimalisering, lokale landingssider og stedsspesifikt innhold — til en investering de fleste bedrifter har råd til." },
];

export default function App() {
  const [menuOpen, setMenuOpen] = useState(false);
  const [faqOpen, setFaqOpen] = useState(-1);
  const [formData, setFormData] = useState({ name: "", email: "", url: "", message: "" });

  return (
    <div style={{ fontFamily: "'Outfit', 'Sora', system-ui, sans-serif", color: "#e8e6e1", background: "#0a0a0b", minHeight: "100vh", overflowX: "hidden" }}>
      <style>{`
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Outfit:wght@300;400;500;600;700&display=swap');
        * { margin: 0; padding: 0; box-sizing: border-box; }
        ::selection { background: #c8ff00; color: #0a0a0b; }
        html { scroll-behavior: smooth; }
        @keyframes fadeUp { from { opacity:0; transform:translateY(40px); } to { opacity:1; transform:translateY(0); } }
        @keyframes slideIn { from { opacity:0; transform:translateX(-20px); } to { opacity:1; transform:translateX(0); } }
        @keyframes pulse { 0%,100% { opacity:1; } 50% { opacity:0.5; } }
        @keyframes grain {
          0%, 100% { transform: translate(0, 0); }
          10% { transform: translate(-5%, -10%); }
          30% { transform: translate(3%, -15%); }
          50% { transform: translate(-10%, 5%); }
          70% { transform: translate(9%, -6%); }
          90% { transform: translate(-7%, 12%); }
        }
        .grain::before {
          content: '';
          position: fixed;
          inset: -50%;
          width: 200%;
          height: 200%;
          background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.03'/%3E%3C/svg%3E");
          pointer-events: none;
          z-index: 9999;
          animation: grain 8s steps(10) infinite;
          opacity: 0.4;
        }
        .nav-link { position: relative; }
        .nav-link::after { content:''; position:absolute; bottom:-2px; left:0; width:0; height:1px; background:#c8ff00; transition: width .3s; }
        .nav-link:hover::after { width:100%; }
        .service-card { transition: all .4s ease; border: 1px solid rgba(255,255,255,0.06); }
        .service-card:hover { border-color: rgba(200,255,0,0.3); transform: translateY(-4px); }
        .case-card { transition: all .3s ease; }
        .case-card:hover { transform: scale(1.02); }
        .cta-btn {
          display: inline-flex; align-items: center; gap: 10px;
          padding: 16px 36px; border-radius: 0; font-size: 14px; font-weight: 600;
          letter-spacing: 0.06em; text-transform: uppercase; text-decoration: none;
          transition: all .3s ease; cursor: pointer; border: none;
        }
        .cta-primary { background: #c8ff00; color: #0a0a0b; }
        .cta-primary:hover { background: #dfff4f; transform: translateY(-2px); box-shadow: 0 8px 30px rgba(200,255,0,0.2); }
        .cta-outline { background: transparent; color: #e8e6e1; border: 1px solid rgba(255,255,255,0.2); }
        .cta-outline:hover { border-color: #c8ff00; color: #c8ff00; }
        .network-card { transition: all .3s; border: 1px solid rgba(255,255,255,0.06); }
        .network-card:hover { border-color: rgba(200,255,0,0.4); background: rgba(200,255,0,0.04); }
        input, textarea {
          width: 100%; padding: 14px 0; font-size: 15px; font-family: inherit;
          background: transparent; border: none; border-bottom: 1px solid rgba(255,255,255,0.15);
          color: #e8e6e1; outline: none; transition: border-color .3s;
        }
        input:focus, textarea:focus { border-bottom-color: #c8ff00; }
        input::placeholder, textarea::placeholder { color: rgba(255,255,255,0.3); }
        textarea { resize: none; min-height: 80px; }
      `}</style>

      <div className="grain" />

      {/* ═══ NAVBAR ═══ */}
      <nav style={{
        position: "fixed", top: 0, left: 0, right: 0, zIndex: 1000,
        padding: "0 clamp(20px, 4vw, 60px)",
        background: "rgba(10,10,11,0.85)", backdropFilter: "blur(20px)",
        borderBottom: "1px solid rgba(255,255,255,0.04)",
      }}>
        <div style={{ maxWidth: 1200, margin: "0 auto", display: "flex", justifyContent: "space-between", alignItems: "center", height: 72 }}>
          <a href="#" style={{ textDecoration: "none", display: "flex", alignItems: "center", gap: 10 }}>
            <div style={{ width: 8, height: 8, background: "#c8ff00", borderRadius: "50%" }} />
            <span style={{ fontSize: 18, fontWeight: 700, color: "#e8e6e1", letterSpacing: "-0.02em" }}>SEOBYRÅ</span>
            <span style={{ fontSize: 10, color: "rgba(255,255,255,0.3)", letterSpacing: "0.05em" }}>.COM</span>
          </a>
          <div style={{ display: "flex", gap: 32, alignItems: "center" }}>
            {["Tjenester", "Resultater", "Nettverk", "Kontakt"].map(item => (
              <a key={item} href={`#${item.toLowerCase()}`} className="nav-link"
                style={{ fontSize: 13, fontWeight: 500, color: "rgba(255,255,255,0.6)", textDecoration: "none", letterSpacing: "0.03em" }}>
                {item}
              </a>
            ))}
            <a href="#kontakt" className="cta-btn cta-primary" style={{ padding: "10px 24px", fontSize: 12 }}>
              Gratis analyse
            </a>
          </div>
        </div>
      </nav>

      {/* ═══ HERO ═══ */}
      <header style={{
        minHeight: "100vh", display: "flex", alignItems: "center",
        padding: "120px clamp(20px, 4vw, 60px) 80px",
        position: "relative", overflow: "hidden",
      }}>
        {/* Ambient bg */}
        <div style={{
          position: "absolute", top: "-20%", right: "-10%", width: "60vw", height: "60vw",
          background: "radial-gradient(circle, rgba(200,255,0,0.04) 0%, transparent 70%)",
          pointerEvents: "none",
        }} />
        <div style={{
          position: "absolute", bottom: "10%", left: "-5%", width: "40vw", height: "40vw",
          background: "radial-gradient(circle, rgba(200,255,0,0.02) 0%, transparent 70%)",
          pointerEvents: "none",
        }} />

        <div style={{ maxWidth: 1200, margin: "0 auto", width: "100%", position: "relative", zIndex: 1 }}>
          <div style={{ animation: "fadeUp .8s ease both" }}>
            <div style={{
              display: "inline-flex", alignItems: "center", gap: 8,
              padding: "6px 16px", border: "1px solid rgba(200,255,0,0.2)", borderRadius: 100,
              marginBottom: 40, fontSize: 12, fontWeight: 500, color: "#c8ff00",
              letterSpacing: "0.04em",
            }}>
              <span style={{ width: 6, height: 6, background: "#c8ff00", borderRadius: "50%", animation: "pulse 2s infinite" }} />
              Norges nye SEO- og AEO-byrå
            </div>
          </div>

          <h1 style={{
            fontFamily: "'Playfair Display', Georgia, serif",
            fontSize: "clamp(3rem, 7vw, 6.5rem)",
            fontWeight: 400, lineHeight: 1.05, letterSpacing: "-0.03em",
            maxWidth: 900,
            animation: "fadeUp .8s ease .1s both",
          }}>
            Vi gjør bedriften din<br />
            <em style={{ fontStyle: "italic", color: "#c8ff00" }}>synlig</em> — i søk<br />
            og i AI
          </h1>

          <p style={{
            fontSize: "clamp(16px, 1.8vw, 20px)", lineHeight: 1.65,
            color: "rgba(255,255,255,0.5)", maxWidth: 540, marginTop: 32,
            animation: "fadeUp .8s ease .2s both",
          }}>
            Søkemotoroptimalisering og AI-søkeoptimalisering for norske bedrifter som vil dominere — ikke bare delta.
          </p>

          <div style={{ display: "flex", gap: 16, marginTop: 48, flexWrap: "wrap", animation: "fadeUp .8s ease .3s both" }}>
            <a href="#kontakt" className="cta-btn cta-primary">
              Bestill gratis synlighetsanalyse →
            </a>
            <a href="#tjenester" className="cta-btn cta-outline">
              Se hva vi gjør
            </a>
          </div>

          {/* Trust bar */}
          <div style={{
            display: "flex", gap: "clamp(32px, 5vw, 64px)", marginTop: 80,
            paddingTop: 40, borderTop: "1px solid rgba(255,255,255,0.06)",
            animation: "fadeUp .8s ease .4s both",
          }}>
            {[
              ["150+", "Søkeord på side 1"],
              ["47", "Aktive kunder"],
              ["340%", "Snitt trafikkvekst"],
              ["8+", "År med SEO-erfaring"],
            ].map(([val, label]) => (
              <div key={label}>
                <div style={{ fontSize: "clamp(24px, 3vw, 36px)", fontWeight: 700, color: "#e8e6e1", letterSpacing: "-0.02em" }}>{val}</div>
                <div style={{ fontSize: 12, color: "rgba(255,255,255,0.35)", marginTop: 4, letterSpacing: "0.02em" }}>{label}</div>
              </div>
            ))}
          </div>
        </div>
      </header>

      {/* ═══ SERVICES ═══ */}
      <section id="tjenester" style={{ padding: "120px clamp(20px, 4vw, 60px)", borderTop: "1px solid rgba(255,255,255,0.04)" }}>
        <div style={{ maxWidth: 1200, margin: "0 auto" }}>
          <Reveal>
            <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-end", marginBottom: 64, flexWrap: "wrap", gap: 24 }}>
              <div>
                <div style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.12em", textTransform: "uppercase", color: "#c8ff00", marginBottom: 16 }}>Tjenester</div>
                <h2 style={{ fontFamily: "'Playfair Display', serif", fontSize: "clamp(2rem, 4vw, 3.2rem)", fontWeight: 400, lineHeight: 1.15, letterSpacing: "-0.02em" }}>
                  Alt du trenger for å<br /><em style={{ fontStyle: "italic" }}>dominere</em> i søk
                </h2>
              </div>
              <p style={{ fontSize: 15, color: "rgba(255,255,255,0.45)", maxWidth: 380, lineHeight: 1.65 }}>
                Vi dekker hele spekteret — fra teknisk grunnlag til AI-optimalisering. Hver tjeneste er designet for å flytte nålen målbart.
              </p>
            </div>
          </Reveal>

          <div style={{ display: "grid", gridTemplateColumns: "repeat(auto-fit, minmax(340px, 1fr))", gap: 1 }}>
            {SERVICES.map((s, i) => (
              <Reveal key={s.num} delay={i * 0.08}>
                <div className="service-card" style={{
                  padding: "40px 36px", background: "rgba(255,255,255,0.015)",
                  minHeight: 260,
                }}>
                  <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start", marginBottom: 20 }}>
                    <span style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.2)", letterSpacing: "0.08em" }}>{s.num}</span>
                    <span style={{ fontSize: 28 }}>{s.icon}</span>
                  </div>
                  <h3 style={{ fontSize: 22, fontWeight: 600, marginBottom: 12, letterSpacing: "-0.01em" }}>{s.title}</h3>
                  <p style={{ fontSize: 14, lineHeight: 1.7, color: "rgba(255,255,255,0.45)" }}>{s.desc}</p>
                </div>
              </Reveal>
            ))}
          </div>
        </div>
      </section>

      {/* ═══ AEO SPOTLIGHT ═══ */}
      <section style={{
        padding: "100px clamp(20px, 4vw, 60px)",
        background: "linear-gradient(180deg, rgba(200,255,0,0.03) 0%, transparent 100%)",
        borderTop: "1px solid rgba(200,255,0,0.08)",
        borderBottom: "1px solid rgba(200,255,0,0.08)",
      }}>
        <div style={{ maxWidth: 1200, margin: "0 auto" }}>
          <Reveal>
            <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "clamp(40px, 6vw, 80px)", alignItems: "center" }}>
              <div>
                <div style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.12em", textTransform: "uppercase", color: "#c8ff00", marginBottom: 16 }}>Ny disiplin</div>
                <h2 style={{ fontFamily: "'Playfair Display', serif", fontSize: "clamp(1.8rem, 3.5vw, 2.8rem)", fontWeight: 400, lineHeight: 1.2, letterSpacing: "-0.02em", marginBottom: 24 }}>
                  AI-søk er her.<br />Er <em style={{ fontStyle: "italic" }}>du</em> synlig?
                </h2>
                <p style={{ fontSize: 15, lineHeight: 1.75, color: "rgba(255,255,255,0.5)", marginBottom: 16 }}>
                  ChatGPT, Perplexity og Google AI Overviews endrer fundamentalt hvordan folk finner informasjon. I stedet for å klikke gjennom ti blå lenker, får brukerne nå ett generert svar — med kilder.
                </p>
                <p style={{ fontSize: 15, lineHeight: 1.75, color: "rgba(255,255,255,0.5)", marginBottom: 32 }}>
                  Vi sørger for at din bedrift er den kilden. Gjennom strukturert data, autoritative kunnskapssider og strategisk innhold bygger vi tilstedeværelsen din i AI-genererte svar — ikke bare i tradisjonelle søkeresultater.
                </p>
                <a href="#kontakt" className="cta-btn cta-primary" style={{ fontSize: 13 }}>Bli synlig i AI-søk →</a>
              </div>
              <div style={{
                background: "rgba(255,255,255,0.03)", border: "1px solid rgba(255,255,255,0.06)",
                borderRadius: 12, padding: 40, position: "relative",
              }}>
                <div style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.3)", letterSpacing: "0.08em", textTransform: "uppercase", marginBottom: 24 }}>AI-søkeresultat — eksempel</div>
                <div style={{ background: "rgba(200,255,0,0.06)", borderRadius: 8, padding: 24, border: "1px solid rgba(200,255,0,0.1)", marginBottom: 16 }}>
                  <div style={{ fontSize: 13, color: "rgba(255,255,255,0.4)", marginBottom: 8 }}>🤖 AI-generert svar</div>
                  <p style={{ fontSize: 14.5, lineHeight: 1.7, color: "rgba(255,255,255,0.75)" }}>
                    «For å forbedre organisk synlighet bør bedrifter fokusere på teknisk SEO, innholdskvalitet og strukturert data...»
                  </p>
                </div>
                <div style={{ fontSize: 12, color: "rgba(255,255,255,0.3)", marginBottom: 8 }}>Kilder:</div>
                <div style={{ display: "flex", flexDirection: "column", gap: 8 }}>
                  <div style={{ display: "flex", alignItems: "center", gap: 10, padding: "10px 14px", background: "rgba(200,255,0,0.08)", borderRadius: 6, border: "1px solid rgba(200,255,0,0.15)" }}>
                    <span style={{ width: 6, height: 6, background: "#c8ff00", borderRadius: "50%" }} />
                    <span style={{ fontSize: 13, fontWeight: 600, color: "#c8ff00" }}>seobyrå.com</span>
                    <span style={{ fontSize: 12, color: "rgba(255,255,255,0.3)" }}>— Din bedrift</span>
                  </div>
                  {["kilde2.no", "kilde3.no"].map(s => (
                    <div key={s} style={{ display: "flex", alignItems: "center", gap: 10, padding: "10px 14px", background: "rgba(255,255,255,0.02)", borderRadius: 6 }}>
                      <span style={{ width: 6, height: 6, background: "rgba(255,255,255,0.15)", borderRadius: "50%" }} />
                      <span style={{ fontSize: 13, color: "rgba(255,255,255,0.3)" }}>{s}</span>
                    </div>
                  ))}
                </div>
              </div>
            </div>
          </Reveal>
        </div>
      </section>

      {/* ═══ RESULTS / CASES ═══ */}
      <section id="resultater" style={{ padding: "120px clamp(20px, 4vw, 60px)", borderTop: "1px solid rgba(255,255,255,0.04)" }}>
        <div style={{ maxWidth: 1200, margin: "0 auto" }}>
          <Reveal>
            <div style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.12em", textTransform: "uppercase", color: "#c8ff00", marginBottom: 16 }}>Resultater</div>
            <h2 style={{ fontFamily: "'Playfair Display', serif", fontSize: "clamp(2rem, 4vw, 3.2rem)", fontWeight: 400, lineHeight: 1.15, letterSpacing: "-0.02em", marginBottom: 64 }}>
              Tall som <em style={{ fontStyle: "italic" }}>snakker</em>
            </h2>
          </Reveal>

          <div style={{ display: "grid", gridTemplateColumns: "repeat(auto-fit, minmax(260px, 1fr))", gap: 16 }}>
            {CASES.map((c, i) => (
              <Reveal key={i} delay={i * 0.1}>
                <div className="case-card" style={{
                  background: "rgba(255,255,255,0.02)", border: "1px solid rgba(255,255,255,0.06)",
                  borderRadius: 2, padding: 36, position: "relative", overflow: "hidden",
                }}>
                  <div style={{
                    position: "absolute", top: 0, left: 0, right: 0, height: 2,
                    background: `linear-gradient(90deg, #c8ff00 ${25 + i * 20}%, transparent)`,
                  }} />
                  <div style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.3)", letterSpacing: "0.08em", textTransform: "uppercase", marginBottom: 20 }}>{c.industry}</div>
                  <div style={{ fontSize: "clamp(36px, 5vw, 52px)", fontWeight: 700, color: "#c8ff00", letterSpacing: "-0.03em", lineHeight: 1 }}>{c.metric}</div>
                  <div style={{ fontSize: 14, fontWeight: 500, marginTop: 8, marginBottom: 4 }}>{c.label}</div>
                  <div style={{ fontSize: 12, color: "rgba(255,255,255,0.3)" }}>{c.period}</div>
                  <div style={{ fontSize: 13, color: "rgba(255,255,255,0.4)", marginTop: 20, lineHeight: 1.55, borderTop: "1px solid rgba(255,255,255,0.06)", paddingTop: 16 }}>{c.detail}</div>
                </div>
              </Reveal>
            ))}
          </div>
        </div>
      </section>

      {/* ═══ PROCESS ═══ */}
      <section style={{ padding: "100px clamp(20px, 4vw, 60px)", background: "rgba(255,255,255,0.01)", borderTop: "1px solid rgba(255,255,255,0.04)" }}>
        <div style={{ maxWidth: 1200, margin: "0 auto" }}>
          <Reveal>
            <div style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.12em", textTransform: "uppercase", color: "#c8ff00", marginBottom: 16 }}>Prosess</div>
            <h2 style={{ fontFamily: "'Playfair Display', serif", fontSize: "clamp(2rem, 4vw, 3.2rem)", fontWeight: 400, lineHeight: 1.15, letterSpacing: "-0.02em", marginBottom: 64 }}>
              Slik jobber vi
            </h2>
          </Reveal>
          <div style={{ display: "grid", gridTemplateColumns: "repeat(auto-fit, minmax(220px, 1fr))", gap: 0 }}>
            {[
              ["01", "Synlighetsanalyse", "Vi kartlegger din nåværende posisjon, konkurrenter, teknisk status og muligheter."],
              ["02", "Strategi", "Basert på analysen bygger vi en skreddersydd SEO- og AEO-strategi med klare KPI-er."],
              ["03", "Implementering", "Vi utfører teknisk optimalisering, innholdsproduksjon og lenkebygging i prioritert rekkefølge."],
              ["04", "Måling & skalering", "Månedlig rapportering med konkrete tall. Vi justerer og skalerer det som fungerer."],
            ].map(([num, title, desc], i) => (
              <Reveal key={num} delay={i * 0.1}>
                <div style={{ padding: "36px 32px", borderLeft: i > 0 ? "1px solid rgba(255,255,255,0.06)" : "none" }}>
                  <div style={{ fontSize: 36, fontWeight: 700, color: "rgba(200,255,0,0.15)", letterSpacing: "-0.03em", marginBottom: 16 }}>{num}</div>
                  <h3 style={{ fontSize: 18, fontWeight: 600, marginBottom: 10 }}>{title}</h3>
                  <p style={{ fontSize: 14, lineHeight: 1.65, color: "rgba(255,255,255,0.4)" }}>{desc}</p>
                </div>
              </Reveal>
            ))}
          </div>
        </div>
      </section>

      {/* ═══ NETWORK ═══ */}
      <section id="nettverk" style={{ padding: "120px clamp(20px, 4vw, 60px)", borderTop: "1px solid rgba(255,255,255,0.04)" }}>
        <div style={{ maxWidth: 1200, margin: "0 auto" }}>
          <Reveal>
            <div style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.12em", textTransform: "uppercase", color: "#c8ff00", marginBottom: 16 }}>Økosystem</div>
            <h2 style={{ fontFamily: "'Playfair Display', serif", fontSize: "clamp(2rem, 4vw, 3.2rem)", fontWeight: 400, lineHeight: 1.15, letterSpacing: "-0.02em", marginBottom: 16 }}>
              Vårt kunnskaps&shy;nettverk
            </h2>
            <p style={{ fontSize: 15, color: "rgba(255,255,255,0.45)", maxWidth: 560, lineHeight: 1.65, marginBottom: 48 }}>
              Vi eier og opererer Norges mest omfattende nettverk av autoritative kunnskapsportaler innen SEO og digital synlighet.
            </p>
          </Reveal>
          <div style={{ display: "grid", gridTemplateColumns: "repeat(auto-fit, minmax(260px, 1fr))", gap: 12 }}>
            {NETWORK.map((n, i) => (
              <Reveal key={n.domain} delay={i * 0.06}>
                <div className="network-card" style={{ padding: "28px 24px", borderRadius: 2, background: "rgba(255,255,255,0.015)", cursor: "default" }}>
                  <div style={{ fontSize: 15, fontWeight: 600, color: "#c8ff00", marginBottom: 4 }}>{n.domain}</div>
                  <div style={{ fontSize: 13, fontWeight: 500, color: "#e8e6e1", marginBottom: 6 }}>{n.label}</div>
                  <div style={{ fontSize: 12.5, color: "rgba(255,255,255,0.35)", lineHeight: 1.5 }}>{n.desc}</div>
                </div>
              </Reveal>
            ))}
          </div>
        </div>
      </section>

      {/* ═══ FAQ ═══ */}
      <section style={{ padding: "100px clamp(20px, 4vw, 60px)", borderTop: "1px solid rgba(255,255,255,0.04)" }}>
        <div style={{ maxWidth: 760, margin: "0 auto" }}>
          <Reveal>
            <div style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.12em", textTransform: "uppercase", color: "#c8ff00", marginBottom: 16 }}>FAQ</div>
            <h2 style={{ fontFamily: "'Playfair Display', serif", fontSize: "clamp(2rem, 4vw, 3.2rem)", fontWeight: 400, lineHeight: 1.15, letterSpacing: "-0.02em", marginBottom: 48 }}>
              Vanlige spørsmål
            </h2>
          </Reveal>
          {FAQ_ITEMS.map((item, i) => (
            <div key={i} style={{ borderBottom: "1px solid rgba(255,255,255,0.06)" }}>
              <button onClick={() => setFaqOpen(faqOpen === i ? -1 : i)} style={{
                width: "100%", display: "flex", justifyContent: "space-between", alignItems: "center",
                padding: "22px 0", background: "none", border: "none", fontFamily: "inherit",
                fontSize: 16, fontWeight: 500, color: "#e8e6e1", cursor: "pointer", textAlign: "left", gap: 20,
              }}>
                {item.q}
                <span style={{ color: "#c8ff00", fontSize: 20, fontWeight: 300, transform: faqOpen === i ? "rotate(45deg)" : "", transition: "transform .3s", flexShrink: 0 }}>+</span>
              </button>
              <div style={{ maxHeight: faqOpen === i ? 300 : 0, overflow: "hidden", transition: "max-height .4s ease" }}>
                <p style={{ paddingBottom: 22, fontSize: 14.5, color: "rgba(255,255,255,0.5)", lineHeight: 1.75 }}>{item.a}</p>
              </div>
            </div>
          ))}
        </div>
      </section>

      {/* ═══ CONTACT / CTA ═══ */}
      <section id="kontakt" style={{
        padding: "120px clamp(20px, 4vw, 60px)",
        background: "linear-gradient(180deg, rgba(200,255,0,0.02) 0%, rgba(10,10,11,1) 100%)",
        borderTop: "1px solid rgba(200,255,0,0.08)",
      }}>
        <div style={{ maxWidth: 1200, margin: "0 auto" }}>
          <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "clamp(40px, 6vw, 100px)", alignItems: "start" }}>
            <Reveal>
              <div>
                <div style={{ fontSize: 12, fontWeight: 600, letterSpacing: "0.12em", textTransform: "uppercase", color: "#c8ff00", marginBottom: 16 }}>Kom i gang</div>
                <h2 style={{ fontFamily: "'Playfair Display', serif", fontSize: "clamp(2rem, 4vw, 3rem)", fontWeight: 400, lineHeight: 1.15, letterSpacing: "-0.02em", marginBottom: 24 }}>
                  Få en gratis<br /><em style={{ fontStyle: "italic" }}>synlighetsanalyse</em>
                </h2>
                <p style={{ fontSize: 15, lineHeight: 1.75, color: "rgba(255,255,255,0.45)", marginBottom: 40 }}>
                  Vi analyserer nettstedet ditt, kartlegger konkurrentene, og gir deg en konkret handlingsplan — helt gratis og uforpliktende. Ingen salgspress, bare ærlige råd.
                </p>
                <div style={{ display: "flex", flexDirection: "column", gap: 20 }}>
                  {[
                    "Teknisk SEO-sjekk av nettstedet ditt",
                    "Konkurranseanalyse for dine viktigste søkeord",
                    "Konkrete anbefalinger for forbedring",
                    "Estimat på potensielt trafikkvekst",
                  ].map(item => (
                    <div key={item} style={{ display: "flex", alignItems: "center", gap: 12 }}>
                      <div style={{ width: 20, height: 20, borderRadius: 4, background: "rgba(200,255,0,0.1)", display: "flex", alignItems: "center", justifyContent: "center", flexShrink: 0 }}>
                        <span style={{ color: "#c8ff00", fontSize: 12, fontWeight: 700 }}>✓</span>
                      </div>
                      <span style={{ fontSize: 14, color: "rgba(255,255,255,0.6)" }}>{item}</span>
                    </div>
                  ))}
                </div>
              </div>
            </Reveal>

            <Reveal delay={0.15}>
              <div style={{
                background: "rgba(255,255,255,0.02)", border: "1px solid rgba(255,255,255,0.06)",
                borderRadius: 2, padding: "40px 36px",
              }}>
                <div style={{ display: "flex", flexDirection: "column", gap: 28 }}>
                  <div>
                    <label style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.3)", letterSpacing: "0.08em", textTransform: "uppercase" }}>Navn</label>
                    <input placeholder="Ditt navn" value={formData.name} onChange={e => setFormData({...formData, name: e.target.value})} />
                  </div>
                  <div>
                    <label style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.3)", letterSpacing: "0.08em", textTransform: "uppercase" }}>E-post</label>
                    <input type="email" placeholder="din@epost.no" value={formData.email} onChange={e => setFormData({...formData, email: e.target.value})} />
                  </div>
                  <div>
                    <label style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.3)", letterSpacing: "0.08em", textTransform: "uppercase" }}>Nettside</label>
                    <input placeholder="https://dinside.no" value={formData.url} onChange={e => setFormData({...formData, url: e.target.value})} />
                  </div>
                  <div>
                    <label style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.3)", letterSpacing: "0.08em", textTransform: "uppercase" }}>Melding (valgfritt)</label>
                    <textarea placeholder="Fortell oss kort om hva du ønsker å oppnå..." value={formData.message} onChange={e => setFormData({...formData, message: e.target.value})} />
                  </div>
                  <button className="cta-btn cta-primary" style={{ width: "100%", justifyContent: "center", padding: "18px 36px", fontSize: 14 }}>
                    Send forespørsel →
                  </button>
                  <p style={{ fontSize: 12, color: "rgba(255,255,255,0.25)", textAlign: "center", lineHeight: 1.5 }}>
                    Vi svarer innen 24 timer. Ingen bindingstid, ingen skjulte kostnader.
                  </p>
                </div>
              </div>
            </Reveal>
          </div>
        </div>
      </section>

      {/* ═══ FOOTER ═══ */}
      <footer style={{
        padding: "60px clamp(20px, 4vw, 60px) 40px",
        borderTop: "1px solid rgba(255,255,255,0.04)",
      }}>
        <div style={{ maxWidth: 1200, margin: "0 auto" }}>
          <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start", flexWrap: "wrap", gap: 40, marginBottom: 40 }}>
            <div>
              <div style={{ display: "flex", alignItems: "center", gap: 10, marginBottom: 16 }}>
                <div style={{ width: 8, height: 8, background: "#c8ff00", borderRadius: "50%" }} />
                <span style={{ fontSize: 18, fontWeight: 700 }}>SEOBYRÅ</span>
                <span style={{ fontSize: 10, color: "rgba(255,255,255,0.3)" }}>.COM</span>
              </div>
              <p style={{ fontSize: 13, color: "rgba(255,255,255,0.3)", maxWidth: 300, lineHeight: 1.6 }}>
                Norges SEO- og AEO-byrå. Vi gjør bedrifter synlige i tradisjonelle søkemotorer og AI-drevne søk.
              </p>
            </div>
            <div style={{ display: "flex", gap: "clamp(32px, 5vw, 64px)", flexWrap: "wrap" }}>
              <div>
                <div style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.25)", letterSpacing: "0.08em", textTransform: "uppercase", marginBottom: 16 }}>Tjenester</div>
                {["Teknisk SEO", "Innholdsstrategi", "AI-søkeoptimalisering", "Lenkebygging", "Lokal SEO"].map(s => (
                  <div key={s} style={{ fontSize: 13, color: "rgba(255,255,255,0.4)", marginBottom: 8, cursor: "pointer" }}>{s}</div>
                ))}
              </div>
              <div>
                <div style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.25)", letterSpacing: "0.08em", textTransform: "uppercase", marginBottom: 16 }}>Nettverk</div>
                {NETWORK.slice(0, 5).map(n => (
                  <div key={n.domain} style={{ fontSize: 13, color: "rgba(255,255,255,0.4)", marginBottom: 8, cursor: "pointer" }}>{n.domain}</div>
                ))}
              </div>
              <div>
                <div style={{ fontSize: 11, fontWeight: 600, color: "rgba(255,255,255,0.25)", letterSpacing: "0.08em", textTransform: "uppercase", marginBottom: 16 }}>Kontakt</div>
                <div style={{ fontSize: 13, color: "rgba(255,255,255,0.4)", marginBottom: 8 }}>hei@seobyrå.com</div>
                <div style={{ fontSize: 13, color: "rgba(255,255,255,0.4)", marginBottom: 8 }}>Oslo, Norge</div>
              </div>
            </div>
          </div>
          <div style={{ borderTop: "1px solid rgba(255,255,255,0.04)", paddingTop: 24, display: "flex", justifyContent: "space-between", flexWrap: "wrap", gap: 12 }}>
            <span style={{ fontSize: 12, color: "rgba(255,255,255,0.2)" }}>© 2026 Seobyrå.com — Alle rettigheter forbeholdt.</span>
            <span style={{ fontSize: 12, color: "rgba(255,255,255,0.15)" }}>En del av <span style={{ color: "rgba(255,255,255,0.35)", fontWeight: 600 }}>IT-FIRMA</span></span>
          </div>
        </div>
      </footer>
    </div>
  );
}
