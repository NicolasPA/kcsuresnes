# Lignée historique des professeurs principaux du Karaté Club de Suresnes

```mermaid
graph TD
    A01["Représentations picuturales d'arts martiaux<br/>(-3000 AEC)<br/>Égypte, Mésopotamie"]
    -.-> A02["Mentions dans les Védas<br/>(-1500 AEC)<br/>Inde"]
    -.-> A03["Mentions dans les Annales des Printemps et Automnes<br/>(-500 AEC)<br/>Chine"]
    -.-> A04["Temple Shaolin: Buddhabhadra, Bodhidharma, Huiguang, Sengchou, Huike <br/>(~500)<br/>Inde → Chine"]
    A02 -.-> A04

    -.-> A05["36 familles Min de Kume<br/>(>1400)<br/>Chine → Okinawa"]
    A04 -.-> A06["Émissaires de l'empire Chinois<br/>(>1400)<br/>Chine → Okinawa"]
    -.-> A07["Noblesse et élite du Royaume des Ryukyu<br/>(1429–1879)<br/>Okinawa"]
    A05 -.-> A07
    A08["Autres influences<br/>(>1300)<br/>Taiwan, Corée, Thailand, Malaisie, Indonésie"]
    A08 -.-> A07

    A04 -.-> A1["Kusanku<br/>(~1700)<br/>Chine"]
    A2["Chatan Yara<br/>(1668–1756)<br/>Okinawa"]
    A07 -.-> A2
    A3["Takahara Pechin<br/>(1683-1760)<br/>Okinawa"]
    A07 -.-> A3
    B1["Kangi Sakugawa<br/>(1733-1815)<br/>Okinawa"]
    A1 --> B1
    A2 --> B1
    A3 --> B1
    --> B2["Kanga Sakugawa<br/>(1786-1867)<br/>Okinawa"]
    --> C["Sokon Matsumura [Shuri-te]<br/>(1797-1889)<br/>Okinawa"]
    --> D["Anko Itosu<br/>(1831-1915)<br/>Okinawa"]
    C --> E["Anko Asato<br/>(1827-1906)<br/>Okinawa"]
    D --> F["Gichin Funakoshi [Shotokan]<br/>(1868-1957)<br/>Okinawa → Tokyo"]
    E --> F
    --> G["Minoru Mochizuki<br/>(1907-2003)<br/>Japon → France"]
    --> H["Hiroo Mochizuki<br/>(1936-)<br/>Japon → France"]
    --> I["Henry Plée<br/>(1923-1997)<br/>France"]
    J["Taïji Kasé<br/>(1929-2004)<br/>Japon → France"]
    F -.-> J
    I --> K["Jean-Pierre Lavorato<br/>(1944-)<br/>France"]
    J --> K
    I --> L["Georges Hernaez<br/>(1941-)<br/>France"]
    G --> L
    H --> L
    J --> L
    L --> M["Pierre Blot<br/>(1954-)<br/>KC Suresnes, France"]
    K --> M
    J --> M
    M --> N["Pascal Pinault<br/>(1961-)<br/>KC Suresnes, France"]
    
    classDef dottedStyle stroke:#333,stroke-dasharray: 5 5,stroke-width:2px
    class A01,A02,A03,A04,A05,A06,A07,A08 dottedStyle
```

<!-- Load Mermaid library from CDN -->
<script src="https://cdn.jsdelivr.net/npm/mermaid@11.14.0/dist/mermaid.min.js"></script>
<!-- Optional: Style Mermaid diagrams -->
<style>
  .mermaid {
    background-color: #f8f9fa; /* Light gray background */
    padding: 1.5rem; /* Add padding around diagrams */
    border-radius: 8px; /* Rounded corners */
    overflow-x: auto; /* Horizontal scroll for wide diagrams */
    margin: 1rem 0; /* Spacing above/below diagrams */
  }
</style>
<!-- Initialize Mermaid and render diagrams -->
<script>
  // Wait for the page to fully load
  document.addEventListener('DOMContentLoaded', function() {
    // Find all Markdown code blocks with class "language-mermaid"
    const mermaidCodeBlocks = document.querySelectorAll('pre code.language-mermaid');
 
    // Convert each code block into a Mermaid diagram
    mermaidCodeBlocks.forEach(block => {
      // Create a new div for Mermaid to render into
      const mermaidDiv = document.createElement('div');
      mermaidDiv.className = 'mermaid'; // Match the CSS class above
      mermaidDiv.textContent = block.textContent; // Copy diagram code
 
      // Replace the original code block with the Mermaid div
      block.parentNode.replaceChild(mermaidDiv, block);
    });
 
    // Initialize Mermaid with default settings
    mermaid.initialize({
      startOnLoad: true, // Render diagrams when Mermaid loads
      theme: 'default', // Use default theme (options: default, dark, forest, neutral)
      logLevel: 3 // Suppress non-critical logs (0 = debug, 3 = error)
    });
  });
</script>
