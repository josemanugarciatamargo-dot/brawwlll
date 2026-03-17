 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
new file mode 100644
index 0000000000000000000000000000000000000000..ba2df58d1259251ab09d7efdc5a6f08bf0751ad0
--- /dev/null
+++ b/README.md
@@ -0,0 +1,26 @@
+# BrawlLite Web (HTML + CSS + JavaScript)
+
+Versión web jugable en **un solo archivo `index.html`** al estilo Brawl Stars.
+
+## Características
+- Menús completos: Jugar, Brawlers, Mejoras, Skins y Tienda de créditos.
+- Guardado/carga automático y manual usando `localStorage`.
+- Copas por brawler y copas totales.
+- Modos de juego: Atrapagemas, Supervivencia Solo y Balón Brawl.
+- Partidas contra bots con fuerza variable.
+- Brawlers con rareza, poder, skins y desbloqueo progresivo.
+- Desbloqueo por:
+  - Camino de copas.
+  - Créditos en tienda.
+- Sistema de mejoras de poder y compra/equipado de skins.
+
+## Ejecutar
+Abre `index.html` directamente en tu navegador.
+
+Opcional con servidor local:
+
+```bash
+python3 -m http.server 8000
+```
+
+Luego entra a `http://localhost:8000`.
 
EOF
)
