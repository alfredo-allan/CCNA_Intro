# 🎯 BRIEFING CCNA MODULE GENERATOR

## 📌 Contexto

* **CSS Global:** `global.css` (já refatorado)
* **Framework:** Bootstrap 5 + FontAwesome
* **Animações:** Anime.js (opcional)

---

## 🧩 Estrutura Obrigatória por Módulo

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NET-ACAD · Módulo X | [Título]</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="../css/global.css">
</head>
<body>
    <!-- NAVBAR (fixa) -->
    <nav class="navbar-glass">
        <div class="container">
            <a class="navbar-brand" href="modulos.html">
                <i class="fas fa-skull"></i>
                Cyber<span style="color: white">Docs</span>
            </a>
            <a href="../index.html" class="btn-cisco-outline">
                <i class="fas fa-arrow-left me-1"></i> Módulos
            </a>
        </div>
    </nav>

    <main class="container py-4">
        <!-- HEADER DO MÓDULO -->
        <div class="text-center mb-4">
            <span class="section-badge">
                <i class="fas fa-cube me-1"></i> Módulo X
            </span>
            <h1 class="display-6 fw-bold">[Título do Módulo]</h1>
            <p class="text-dim">Introduction to Networks (ITN) · Cisco CCNAv7</p>
        </div>

        <!-- ÍNDICE RÁPIDO (opcional, por seção) -->
        <div class="content-card mb-4">
            <h3 class="cisco-subtitle">
                <i class="fas fa-list me-2"></i> Navegação rápida
            </h3>
            <div class="row">
                <div class="col-md-6">
                    <ul class="list-unstyled">
                        <li><a href="#secao-X-Y" class="text-dim">
                            <i class="fas fa-chevron-right me-2" style="color: var(--cisco-green)"></i>X.Y Título
                        </a></li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- SEÇÕES DO MÓDULO -->
        <div id="secao-X-Y" class="content-card">
            <span class="section-badge">X.Y Subtítulo</span>
            <h2 class="cisco-title">Título Principal</h2>
            <p>Conteúdo teórico...</p>
            
            <!-- Tabela comparativa -->
            <div class="table-responsive">
                <table class="table table-cisco">
                    <thead>
                        <tr><th>Coluna 1</th><th>Coluna 2</th></tr>
                    </thead>
                    <tbody>
                        <tr><td>Dado 1</td><td>Dado 2</td></tr>
                    </tbody>
                </table>
            </div>
            
            <!-- Terminal Cisco -->
            <div class="ios-terminal">
                <pre><code>Router# show running-config</code></pre>
            </div>
            
            <!-- Alertas -->
            <div class="alert-cisco">
                <i class="fas fa-info-circle me-2"></i> Informação importante
            </div>
            
            <!-- Imagem com fallback -->
            <img src="images/moduloX/exemplo.png" class="content-img w-100"
                 alt="Descrição" onerror="this.style.display='none'">
        </div>

        <!-- QUIZ INTERATIVO (padronizado) -->
        <div class="content-card">
            <h3 class="cisco-subtitle">
                <i class="fas fa-quiz me-2"></i> Verifique seu aprendizado
            </h3>
            <p><strong>[Pergunta]</strong></p>
            <div class="quiz-option" onclick="document.getElementById('q1').checked = true">
                <input type="radio" name="quiz" id="q1" value="correta">
                <label>Opção correta</label>
            </div>
            <div class="quiz-option" onclick="document.getElementById('q2').checked = true">
                <input type="radio" name="quiz" id="q2" value="errada">
                <label>Opção errada</label>
            </div>
            <button class="btn-check-answer mt-2" onclick="checkQuiz()">
                Verificar resposta
            </button>
            <div id="quizResposta" class="quiz-answer mt-2" style="display: none"></div>
        </div>
    </main>

    <!-- FOOTER PADRÃO -->
    <footer class="cisco-footer">
        <div class="container text-center">
            <i class="fas fa-skull me-2" style="color: var(--cisco-green)"></i>
            <strong>Cisco Cyber Docs</strong> · Módulo X - [Título]
        </div>
    </footer>

    <!-- SCRIPT PADRÃO DE QUIZ -->
    <script>
        function checkQuiz() {
            const radios = document.getElementsByName('quiz');
            let selected = null;
            for (let r of radios) if (r.checked) { selected = r.value; break; }
            const div = document.getElementById('quizResposta');
            div.style.display = 'block';
            if (selected === 'correta') {
                div.className = 'quiz-answer correct';
                div.innerHTML = '<i class="fas fa-check-circle me-2"></i> Correto! [Explicação]';
            } else if (selected) {
                div.className = 'quiz-answer incorrect';
                div.innerHTML = '<i class="fas fa-times-circle me-2"></i> Incorreto. [Explicação]';
            } else {
                div.className = 'quiz-answer incorrect';
                div.innerHTML = '<i class="fas fa-exclamation-triangle me-2"></i> Selecione uma resposta.';
            }
        }
    </script>
</body>
</html>
```

---

## 🎨 Classes CSS Disponíveis (`global.css`)

| Classe                   | Uso                           |
| ------------------------ | ----------------------------- |
| `.content-card`          | Card principal de conteúdo    |
| `.cisco-title`           | Título com borda verde        |
| `.cisco-subtitle`        | Subtítulo em verde            |
| `.section-badge`         | Badge de seção (Módulo X.Y)   |
| `.table-cisco`           | Tabela estilizada             |
| `.ios-terminal`          | Terminal de comandos Cisco    |
| `.alert-cisco`           | Alerta informativo            |
| `.content-img`           | Imagem com borda e hover      |
| `.quiz-option`           | Opção de quiz interativo      |
| `.btn-check-answer`      | Botão de verificar quiz       |
| `.quiz-answer.correct`   | Resposta correta (verde)      |
| `.quiz-answer.incorrect` | Resposta incorreta (vermelha) |
| `.cisco-footer`          | Rodapé padrão                 |
| `.navbar-glass`          | Navbar fixa com blur          |
| `.btn-cisco-outline`     | Botão outline verde           |
| `.display-6`             | Título principal do módulo    |
| `.text-dim`              | Texto secundário/cinza        |
| `.ipv6-badge`            | Badge para IPv6               |
| `.packet-stack`          | Pilha de protocolos           |
| `.config-step`           | Passo a passo numerado        |

---

## ✅ Checklist para cada página de módulo

* [ ] Usar `global.css` (**NÃO incluir `<style>` interno**)
* [ ] Navbar com `.navbar-glass` + link voltar
* [ ] Header com `.section-badge` + `.display-6` + `.text-dim`
* [ ] Índice rápido (opcional, com links `#secao-X-Y`)
* [ ] Seções com `id="secao-X-Y"` e classe `.content-card`
* [ ] Subtítulos com `.cisco-subtitle`
* [ ] Tabelas com `.table-cisco` + `.table-responsive`
* [ ] Comandos Cisco dentro de `.ios-terminal`
* [ ] Alertas com `.alert-cisco`
* [ ] Imagens com `.content-img` e `onerror`
* [ ] Quiz padronizado com radio buttons + função `checkQuiz()`
* [ ] Footer com `.cisco-footer`
* [ ] Script de quiz customizado para cada pergunta
