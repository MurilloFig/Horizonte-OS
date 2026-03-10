# 🌌 Horizon OS - Guia Completo do Enigma

Bem-vindo ao simulador **Horizon OS**, uma experiência de Escape Room digital inspirada no Windows XP. Este documento contém toda a documentação do sistema, a narrativa e a resolução passo a passo de todos os puzzles.

---

## 🛠️ Funcionalidades do Sistema

O Horizon OS simula um ambiente de desktop funcional com:
- **Gerenciamento de Arquivos:** Criar, editar, excluir e proteger arquivos `.txt` com senha.
- **Persistência:** O estado do sistema (arquivos criados, puzzles resolvidos) é salvo no `localStorage`.
- **Interface XP:** Botão Iniciar funcional, menu de contexto (botão direito), lixeira e janelas arrastáveis.
- **Navegador Web:** "Horizon Explorer" que requer conexão Wi-Fi.

---

## 🧩 Guia do Enigma (Walkthrough)

O objetivo final é descobrir o segredo do Dr. Valenko e estabilizar o sistema Horizon.

### Passo 1: O Acesso Inicial
1. Abra o aplicativo **External Device** no desktop.
2. Insira o código do pendrive físico: `VX-117-A`.
3. **Resultado:** A pasta **Audio** aparecerá piscando na área de trabalho.

### Passo 2: O Sinal Criptográfico
1. Entre na pasta **Audio** e abra o **Signal Player**.
2. Clique no ícone de gráfico (**Spectral View**) ao lado do botão Play.
3. Dê Play no áudio "Áudio Pen-drive.m4a".
4. Observe as partículas no analisador espectral; elas formarão a palavra **VALENKO**.
5. Digite `VALENKO` no campo "Decoded Text" do player e clique em Verificar.
6. **Resultado:** A pasta **Archive** será desbloqueada no desktop.

### Passo 3: Mapeamento Estelar
1. Abra a pasta **Archive** e inicie o **Star Map 360**.
2. Use as setas do teclado para navegar pelo céu noturno.
3. Insira as coordenadas encontradas nos registros do Dr. Valenko:
   - **RA:** `18.36`
   - **DEC:** `42.11`
4. Clique em **Lock Coordinates**.
5. **Resultado:** O ícone do **Observatory Control** aparecerá no desktop.

### Passo 4: Alinhamento do Observatório
1. Abra o **Observatory Control**.
2. Use o slider para ajustar a inclinação do telescópio para **62°**.
3. Clique em **Start Alignment**.
4. **Resultado:** O executável **MiniGame.exe** (Asteroids) aparecerá no desktop.

### Passo 5: O Filtro de Interferência
1. Abra o **MiniGame.exe** e destrua 100 asteroides para limpar a frequência.
2. Após vencer, você receberá a primeira parte da chave: `OBSERVER`.
3. (Lore) A segunda parte, `FILTER`, deve ser encontrada fisicamente ou deduzida pelos arquivos do sistema.
4. Abra o **Filter Console** (Terminal).
5. Digite o comando final: `EXPLORE OBSERVER-FILTER`.
6. **Resultado:** O sistema será estabilizado e a narrativa final será revelada.

---

## 💻 Comandos do Console (Terminal)

O **Filter Console** (CMD) permite interagir com o sistema em um nível mais profundo. Digite os comandos abaixo para navegar:

- `HELP`: Lista os comandos básicos disponíveis.
- `LS`: Lista todos os arquivos e diretórios visíveis no sistema de arquivos virtual.
- `CAT <nome_do_arquivo>`: Lê o conteúdo de um arquivo de texto diretamente no terminal.
- `CLEAR`: Limpa o histórico de mensagens do console.
- `CONNECT WIFI`: Verifica o status atual da conexão sem fio.
- `SUDO`: Solicita privilégios de administrador (Senha: `ASTRONOMIA`).
- `EXPLORE <keyword>`: O comando mestre para inserir as chaves finais e desbloquear a conclusão do jogo. (Ex: `EXPLORE OBSERVER-FILTER`).

---

## 🔑 Lista de Chaves e Senhas

| Elemento | Chave / Senha |
| :--- | :--- |
| **External Device** | `VX-117-A` |
| **Registro_Espectral_004.log** | `VALENKO1980` |
| **Anomalia_Vectorial.md** | `ORION` |
| **Wi-Fi (SSID: Valenko_Lab)** | `STARGAZER` |
| **Signal Decoder** | `VALENKO` |
| **Star Map (Coordenadas)** | `18.36` / `42.11` |
| **Observatory (Inclinação)** | `62` |
| **Terminal (Sudo/Admin)** | `ASTRONOMIA` |
| **Comando Final** | `EXPLORE OBSERVER-FILTER` |

---

## 📝 Notas de Desenvolvimento
O sistema foi construído utilizando HTML5, Tailwind CSS e Vanilla JavaScript. Toda a lógica de partículas e o motor de física do minigame rodam nativamente no Canvas API.

**Horizon OS v1.0** - Identidade Digital Dr. Valenko.
