# **🌟 Ferramenta de Criação Vetorial - Projeto de Design Moderno e Poderoso**  

![Banner do Projeto](https://imgur.com/lKWZfug.png)  

---

## **🚀 Visão Geral**  

Bem-vindo ao repositório oficial da **Ferramenta de Criação Vetorial**, uma solução de design vetorial de código aberto, moderna e altamente personalizável, desenvolvida em **Python 3.12+**. Este projeto é destinado a designers, desenvolvedores e entusiastas que buscam uma ferramenta flexível e poderosa para criação de gráficos vetoriais com suporte a exportação em múltiplos formatos, incluindo **PNG, JPG, JSON, XML e SVG**.  

Nosso objetivo é oferecer uma experiência de usuário intuitiva, inspirada em softwares profissionais como **Adobe Illustrator** e **CorelDRAW**, mas com a flexibilidade e personalização que só um projeto de código aberto pode proporcionar.  

---

## **🎯 Destaques do Projeto**  

✅ **Design Moderno e Personalizável** – Interface gráfica estilizada e altamente customizável.  
✅ **Exportação em Múltiplos Formatos** – PNG, JPG, JSON, XML e SVG.  
✅ **Suporte a Efeitos Avançados** – Gradientes complexos, sombras, blur, transparências e muito mais.  
✅ **Arquitetura Modular** – Fácil extensão e manutenção.  
✅ **Multiplataforma** – Compatível com Windows, Linux e Mac.  
✅ **Documentação Completa** – Guias de usuário, tutoriais e exemplos práticos.  

---

## **✨ Por Que Escolher Esta Ferramenta?**  

- **Código Aberto:** Totalmente transparente e customizável.  
- **Performance:** Utiliza técnicas de renderização assíncrona e multi-threading para garantir fluidez.  
- **Flexibilidade:** Exporte seus projetos em formatos rasterizados ou estruturados para uso em jogos, sites e outras aplicações.  
- **Comunidade Ativa:** Colabore com outros desenvolvedores e designers para melhorar a ferramenta.  

---

## **📂 Estrutura do Projeto**  

Aqui está a estrutura detalhada do projeto, organizada para facilitar o desenvolvimento e a colaboração:  

```
/VectorTool
 ├── /src/                   # Código-fonte principal
 │   ├── main.py             # Ponto de entrada do aplicativo
 │   ├── ui/                 # Módulos de interface gráfica
 │   │   ├── main_window.py  # Janela principal da aplicação
 │   │   ├── toolbar.py      # Barra de ferramentas personalizável
 │   │   ├── properties_panel.py # Painel de propriedades dos objetos
 │   │   ├── layers_panel.py # Gerenciador de camadas
 │   ├── core/               # Lógica de manipulação de objetos vetoriais
 │   │   ├── shapes.py       # Formas básicas (retângulos, elipses, etc.)
 │   │   ├── bezier.py       # Curvas Bézier e B-spline
 │   │   ├── text.py         # Manipulação de texto
 │   │   ├── effects.py      # Efeitos avançados (sombras, gradientes, etc.)
 │   ├── render/             # Renderização de objetos
 │   │   ├── renderer.py     # Motor de renderização principal
 │   │   ├── skia_renderer.py # Renderização usando Skia
 │   │   ├── cairo_renderer.py # Renderização usando Cairo
 │   ├── storage/            # Salvamento e carregamento de projetos
 │   │   ├── json_handler.py # Manipulação de arquivos JSON
 │   │   ├── xml_handler.py  # Manipulação de arquivos XML
 │   │   ├── project_manager.py # Gerenciador de projetos
 │   ├── utils/              # Funções auxiliares
 │   │   ├── color_utils.py  # Manipulação de cores
 │   │   ├── math_utils.py   # Funções matemáticas para gráficos
 │   │   ├── file_utils.py   # Manipulação de arquivos
 │   ├── assets/             # Recursos visuais (ícones, fonts, etc.)
 ├── /projects/              # Pasta padrão para salvar projetos
 ├── /tests/                 # Testes unitários e de integração
 ├── /docs/                  # Documentação do projeto
 │   ├── user_guide.md       # Guia do usuário
 │   ├── api_reference.md    # Referência da API para desenvolvedores
 │   ├── tutorials/          # Tutoriais passo a passo
 ├── requirements.txt        # Dependências do projeto
 ├── README.md               # Documentação principal
 ├── LICENSE                 # Licença do projeto (MIT)
 ├── .gitignore              # Arquivos ignorados pelo Git
 ├── setup.py                # Script de instalação
 ├── pyproject.toml          # Configuração do Poetry (opcional)
```

---

## **🛠️ Tecnologias Utilizadas**  

### **🔹 Linguagem Principal**  
- **Python 3.12+** – Escolhido por sua simplicidade, performance e vasta biblioteca de suporte.  

### **🔹 Frameworks e Bibliotecas**  
- **Interface Gráfica:** [PyQt6](https://www.riverbankcomputing.com/software/pyqt/) ou [PySide6](https://wiki.qt.io/Qt_for_Python) para uma UI moderna e responsiva.  
- **Renderização Vetorial:** [Skia](https://skia.org/) ou [Cairo](https://www.cairographics.org/) para renderização de alta performance.  
- **Manipulação de Dados:** JSON e XML para armazenamento estruturado.  
- **Gerenciamento de Dependências:** [Poetry](https://python-poetry.org/) para um ambiente de desenvolvimento consistente.  
- **Testes:** [Pytest](https://docs.pytest.org/) para testes unitários e de integração.  

---

## **🎨 Design e Personalização**  

### **🔹 Interface Gráfica Moderna**  
- **Temas Personalizáveis:** Escolha entre temas claros, escuros ou crie o seu próprio.  
- **Layout Flexível:** Rearranje painéis e barras de ferramentas conforme sua preferência.  
- **Ícones e Fontes:** Utilize ícones modernos e fontes personalizadas para uma experiência única.  

### **🔹 Exemplo de Tema Escuro**  
```python
# Exemplo de configuração de tema escuro
app.setStyleSheet("""
    QMainWindow {
        background-color: #2E3440;
        color: #D8DEE9;
    }
    QToolBar {
        background-color: #3B4252;
        border: none;
    }
    QMenuBar {
        background-color: #3B4252;
        color: #D8DEE9;
    }
""")
```

---

## **📝 Exemplo de Estrutura JSON**  

Aqui está um exemplo detalhado de como os projetos serão armazenados em formato JSON:  

```json
{
   "project_name": "MeuProjeto",
   "canvas_size": {
       "width": 2048,
       "height": 2048
   },
   "objects": [
       {
           "type": "rectangle",
           "x": 100,
           "y": 200,
           "width": 300,
           "height": 150,
           "color": "#FF0000",
           "opacity": 0.8,
           "shadow": {
               "enabled": true,
               "color": "#000000",
               "blur": 10,
               "offset_x": 5,
               "offset_y": 5
           }
       },
       {
           "type": "text",
           "x": 50,
           "y": 100,
           "text": "Olá Mundo!",
           "font": "Arial",
           "size": 24,
           "color": "#000000",
           "gradient": {
               "enabled": true,
               "colors": ["#FF0000", "#00FF00"],
               "angle": 45
           }
       }
   ]
}
```

---

## **🚀 Como Contribuir**  

1. **Faça um fork do repositório.**  
2. **Crie uma branch** para sua feature (`git checkout -b feature/nova-feature`).  
3. **Commit suas alterações** (`git commit -m 'Adicionando nova feature'`).  
4. **Push para a branch** (`git push origin feature/nova-feature`).  
5. **Abra um Pull Request** e descreva suas alterações.  

---

## **📜 Licença**  

Este projeto está licenciado sob a **MIT License**. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.  

---

## **📞 Contato**  

Se você tiver dúvidas, sugestões ou quiser colaborar, sinta-se à vontade para entrar em contato:  

- **Email:** ofc.rede@gmail.com 
- **GitHub:** [@seuusuario](https://github.com/LucasDesignerF)  
- **Discord:** lrfortes 

---

**🌟 Vamos construir algo incrível juntos!** 🚀
