# 🌐 BRIEFING TÉCNICO: Projeto NET-ACAD CCNA1

---

## 1. 🎯 VISÃO GERAL DO PROJETO

* **PROJETO:** Documentação Interativa CCNA v7.0 (ITN)
* **BASE DE CONHECIMENTO:** 🌐 NET-ACAD | Introdução a Redes
* **PÚBLICO-ALVO:** Estudantes de Engenharia, TI e Aspirantes a Certificação CCNA
* **TOM VISUAL:** Industrial/Tech (Identidade Cisco Enterprise)
* **ESTRUTURA:** 17 módulos (conforme currículo oficial CCNA1)
* **LOGOTIPO:** NETCORE (Sugerido para diferenciar do CyberSec)

---

## 2. 🎨 IDENTIDADE VISUAL (Ajustes de Acento)

Mantemos o CSS consolidado (`styles.css`), com foco nos seguintes elementos:

### 🎯 Cores de Status (Interface de Redes)

```css
--cisco-green: #66bf53;   /* Link Up / Success */
--accent-blue: #0d6efd;   /* Configuração / Cisco IOS */
--accent-yellow: #ffc107; /* STP Blocking / Warning */
--accent-red: #dc3545;    /* Link Down / Critical */
```

---

## 3. 🧱 COMPONENTES ESPECÍFICOS PARA REDES

O `styles.css` deve suportar as seguintes classes:

| Classe           | Uso               | Descrição                                           |
| ---------------- | ----------------- | --------------------------------------------------- |
| `.ios-terminal`  | Comandos Cisco    | Card preto, texto verde ou branco, prompt `Router#` |
| `.packet-stack`  | Camada OSI/TCP-IP | Grid vertical mostrando o encapsulamento da PDU     |
| `.topology-card` | Diagramas de Rede | Fundo sutil com grid (blueprint)                    |
| `.ipv6-badge`    | Endereçamento     | Destaque para endereços hexadecimais                |
| `.config-step`   | Passo a passo     | Lista numerada com borda lateral                    |

---

## 4. 🗺️ ESTRUTURA DE MÓDULOS (CCNA 1 - ITN)

1. Redes Atuais
2. Configuração de Switch e Dispositivos Finais
3. Protocolos e Modelos (OSI/TCP-IP)
4. Camada Física
5. Sistemas de Numeração (Binário/Hex)
6. Camada de Enlace de Dados
7. Comutação Ethernet
8. Camada de Rede
9. Resolução de Endereço (ARP)
10. Configuração Básica de Roteador
11. Endereçamento IPv4 (Subnetting)
12. Endereçamento IPv6
13. ICMP
14. Camada de Transporte (TCP/UDP)
15. Camada de Aplicação
16. Fundamentos de Segurança de Rede
17. Construir uma Pequena Rede

---

## 5. 🏗️ TEMPLATE DE SEÇÃO (Exemplo CCNA)

```html
<section id="tcp-vs-udp">
  <h2 class="cisco-title display-6 mb-4">14.1 TCP e UDP</h2>
  
  <div class="content-card">
    <h3 class="cisco-subtitle">Comparação de Protocolos</h3>
    <p>Diferenças fundamentais entre entrega confiável e entrega rápida.</p>
    
    <div class="table-responsive">
      <table class="table table-cisco">
        <thead>
          <tr><th>Característica</th><th>TCP</th><th>UDP</th></tr>
        </thead>
        <tbody>
          <tr><td>Conexão</td><td>Orientado a Conexão</td><td>Sem Conexão</td></tr>
          <tr><td>Confiabilidade</td><td>Garantida (Reenvio)</td><td>Melhor Esforço</td></tr>
        </tbody>
      </table>
    </div>
    
    <div class="terminal-card">
      <small class="text-muted">// Verificando conexões ativas no roteador</small>
      <pre><code>Router# show ip sockets</code></pre>
    </div>
  </div>
</section>
```

---

## 6. 🔧 COMANDO PARA O CHAT (Otimizado)

> "Continuando o projeto de documentação NET-ACAD CCNA com o estilo consolidado.
> Contexto: Módulo [X] do curso Introdução a Redes.
> Classes: `.ios-terminal` para comandos, `.table-cisco` para comparativos, `.content-card` para teoria.
> Preciso criar a seção [TÓPICO] com foco em [DETALHE TÉCNICO]."

---

## ✅ OBSERVAÇÕES FINAIS

* Estrutura pensada para documentação técnica escalável
* Compatível com renderização em GitHub / GitLab / Docs estáticos
* Pronto para integração com frameworks como **Next.js**, **VuePress** ou **Docusaurus**
* Segue padrão visual inspirado em documentação enterprise

---

**Versão:** 1.0
**Formato:** Markdown (.md)
**Objetivo:** Base estruturada para documentação interativa CCNA
