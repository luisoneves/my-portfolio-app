## 🖼️ Geração de Imagens
Para otimizar novas imagens:
1. Instale o plugin: `npm install vite-plugin-image-presets`
2. Rode o build: `npm run build`
3. (Opcional) Remova o plugin após gerar os arquivos.

## 🖼️ Otimização de Imagens

### **Comandos Úteis (ImageMagick)**
| Descrição | Comando |
|-----------|---------|
| Converter JPEG → WebP | `magick mogrify -format webp -quality 85 *.jpg` |
| Redimensionar para Full HD | `magick mogrify -resize 1920x *.jpg` |
| Gerar fallback PNG | `magick mogrify -format png *.webp` |

### **Upscale com IA**
- **Waifu2x (online)**: [Link](https://waifu2x.udp.jp/)
- **Real-ESRGAN (CLI)**:
  ```bash
  pip install realesrgan
  realesrgan -i input.jpg -o output.png -n RealESRGAN_x4plus


---

## **📂 Onde Guardar Essas Dicas?**
1. **`README.md`** (recomendado):
   - Visível para todos no repositório (GitHub/GitLab).
   - Fácil de manter atualizado.

2. **Documentação interna** (se o projeto for complexo):
   - Crie um `/docs/` com arquivos como `IMAGE_OPTIMIZATION.md`.

3. **Comentários no código**:
   - Adicione notas em scripts de build (ex.: `vite.config.js`).

---

## **🎯 Conclusão**
- **Para upscale**: Use **Real-ESRGAN** (CLI) ou **Waifu2x** (online).
- **Documente no `README.md`** as principais dicas de otimização.
- **Mantenha as dependências de upscale separadas** (só instale quando precisar).

Exemplo de `README.md` organizado:
```markdown
# Meu Portfólio

## 🛠 Desenvolvimento
- `pnpm install`
- `pnpm run dev`

## 🖼️ Otimização de Imagens
[Veja o guia completo aqui](./docs/IMAGE_OPTIMIZATION.md)


# Meu Portfólio

Portfólio pessoal utilizando Parcel e PNPM, estrutura modular com componentes reutilizáveis e organização otimizada para escalabilidade.

## 🚀 Tecnologias
- Parcel
- PNPM
- Sass (em breve)
- JavaScript

## 📁 Estrutura
Organizado por seções, componentes e dados em JSON para facilitar manutenção e escalabilidade.

## 📦 Instalação
```bash
pnpm install
pnpm run dev
