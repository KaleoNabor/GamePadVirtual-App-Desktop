# 🎮 GamePadVirtual - Controle para Jogos no PC com Streaming

Transforme seu smartphone Android em um controle profissional para PC com streaming de áudio e vídeo de baixa latência. Com ele a falta de controles para jogar com seus amigos ou até mesmo sozinho não será mais um problema, podendo conectar até 8 controles (8 celulares).

---

## 📱+🖥️ COMO UTILIZAR:

- Usar como um controle:
   1. Baixe e Instale o App e o Programa de Windows Disponíveis abaixo
   2. Abra o App no celular e no computador, e conecte-os no mesmo Roteador (Wi-fi + Cabo ou Wi-fi + Wi-fi)
   3. Com o programa no PC aberto, vá no App e clique em "Conectar na Rede" e selecione o Dispositivo que aparecer
   4. Depois no App clique em "Ir para o Controle" e aproveite

- Função de Gamepad Externo:
   1. Conecte o gamepad externo USB ao celular
   2. Abra o App, e as funções dos botões virtuais já serão substituídas pelo gamepad externo
   3. É possível definir os gatilhos para Digitais na barra lateral de configurações na tela de controle quando o Externo estiver conectado.

- Função de Stream da tela do PC:
   1. Escolha o modo de Straming de tela que deseja e aperte em "Aplicar alterações" se modificou algo 
   2. No PC a opção de Iniciar Transmissão, no menu Config de Streaming, precisa estar ativa
   2. No app, assim que ele conectar na rede, na tela de controle, a opção de Assistir Stream já aparecerá no canto superior direito
   3. Você pode alterar o modo de visualização para Imersivo (Tela cheia)(para quem possui um gamepad externo), Split (Tela reduzida para caber os botões fora da Exibição)

---

## 📦 **Downloads**

### 📱 Aplicativo Android
**Versão:** Mais atual  
**Plataforma:** Android 8.0+  
**Arquivo:** `GamePadVirtual-Android-v-.-.-.apk`  
[📥 Baixar APK](https://github.com/KaleoNabor/GamePadVirtual-App-Desktop/releases/download/v1.3.3-APP/GamePadVirtual-v1.3.3.apk)

### 🖥️ Servidor PC
**Versão:** Mais atual  
**Plataforma:** Windows 10/11 (64-bit)  
**Arquivo:** `GamePadVirtual-Server-v-.-.-.zip`  
[📥 Baixar Servidor](https://github.com/KaleoNabor/GamePadVirtual-App-Desktop/releases/download/v1.3.4-Server/GamePadVirtual-Desktop-v1.3.4.zip)

### 🛠️ Drivers Necessários  
**Plataforma:** Windows 10/11 (64-bit)  
**Arquivo:** `drivers.zip`  
[📥 Baixar Drivers](https://github.com/KaleoNabor/GamePadVirtual-App-Desktop/releases/download/v1.3.4-Server/drivers.zip)

---

## ⚙️ Instalação Rápida

### 🔵 Pré-requisito Obrigatório (PC)
Visual C++ Redistributable 2015-2022  
📥 Download Direto Microsoft: https://aka.ms/vs/17/release/vc_redist.x64.exe

### 📋 Passo a Passo
1. 🔵 Instale o VC++ Redist no PC (como Administrador)
2. 📥 Baixe o servidor e extraia o ZIP
3. ✅ Baixe e instale os drivers necessários (Download das versões utilizadas acima):
   - Driver ViGEmBus: O instalador está na pasta \drivers\ViGEmBus_Setup_X.X.X.exe
   - Virtual Display Driver: Abra o arquivo VDD Control.exe em \drivers\VDD.Control.25.7.23\ e clique na opção Install Driver. Quando terminar pode fechar. OBSERVAÇÃO: Instale ele de forma padrão, para pleno funcionamento do sistema de telas virtuais, o programa conta com a estrutura de pastas: C:\VirtualDisplayDriver\vdd_settings.xml
4. 🖥️ Execute GamePadVirtualLauncher.exe
5. 📱 Instale o app no celular
6. 🔍 Conecte na mesma rede e no app aperte "Conectar na Rede"
7. 🎮 Clique em "Ir para o Controle" e está pronto para jogar!

---

## 🚀 Funcionalidades Principais - COMPLETO

### 🎯 Controle Universal Multi-Plataforma
- Emulação Xbox 360 & DualShock 4 via ViGEmBus
- Reconhecimento nativo pelo Windows e jogos
- Suporte a controles físicos via Bluetooth/OTG
- Multitouch com até 8 toques simultâneos
- Controles do PC: Touchpad (mouse) e teclado virtual

### 🖥️ Streaming de Vídeo & Áudio (Alta Performance)
- Captura direta da tela via DirectX 11 (Zero-Copy)
- Codificação hardware acelerada: NVIDIA NVENC, AMD AMF
- Codecs suportados: H.265, H.264, VP8
- Handshake que passa para o computador o que é suportado pelo celular e carrega a transmissão de acordo
- Sistema de fallback inteligente: Automaticamente seleciona codec compatível se H.265 falhar
- Controle de Keyframes: Otimizado para auto-recuperação rápida após instabilidade
- Áudio do sistema de alta fidelidade via WASAPI com roteamento dedicado
- Baixíssima latência com buffers otimizados para sincronia áudio/vídeo perfeita
- Roteamento de áudio inteligente no Android: Detecta fones (com fio/Bluetooth) e alterna automaticamente.

### 📡 Conexão Híbrida & Estabilidade
- Wi-Fi automático com descoberta de rede
- Ancoragem USB para máxima estabilidade
- TCP/UDP otimizado para dados e vídeo
- Reconeção automática se a conexão cair
- Sistema de "Conexão Imortal":
    - Serviço de primeiro plano Android com notificação persistente
    - Sistema de Heartbeat (Ping-Pong) mantém conexão ativa mesmo em segundo plano

### 🎮 Motion Controls para Emuladores
- Servidor DSU nativo (porta 26760)
- Compatibilidade total com Cemu, Yuzu, Ryujinx, Dolphin (Somente por controle de PS4)
- Giroscópio e acelerômetro de alta precisão
- Mira por movimento em jogos compatíveis

### 🛠️ Ferramentas Avançadas
- Editor de layout arrastar-e-soltar
- Touchpad para controle do mouse
- Teclado virtual completo
- Vibração háptica local e remota

### 🖥️ 🎉 SISTEMA DE MONITOR VIRTUAL (NOVO!)
- 🖥️ Resolução Dinâmica e Exata (Modo Um Jogador)
  - Lê a resolução nativa do celular (ex: 1604x720 ou 2400x1080) durante o Handshake
  - Cria um monitor virtual sob medida para o dispositivo
  - Resultado: Imersão total no celular, sem bordas pretas laterais ou esticamento de imagem

- 🎮 Modo Galera (1080p Fixo)
  - Cria um monitor com resolução de 1920x1080 fixa para disponibilizar para todos os jogadores
  - Ideal para múltiplos celulares ou espelhamento em TV
  - Garante o padrão 16:9 universal

- ⚙️ Automação de Arquivos (XML)
  - Edita e reescreve automaticamente o arquivo vdd_settings.xml na pasta do driver
  - Não é mais necessário editar o arquivo de configurações do drive manualmente

- 🔄 Reinício Robusto via PowerShell
  - Comandos nativos do Windows (Get-PnpDevice / Disable / Enable) via PowerShell
  - Driver reinicia corretamente (tela pisca) para aplicar novas configurações

- 🔨 Força Bruta de Resolução (API Windows)
  - Implementação da função ChangeDisplaySettingsExW
  - Força o Windows a aceitar a resolução customizada do XML imediatamente

- 🧠 Cache Inteligente (Anti-Loop)
  - Sistema lembra a última configuração aplicada
  - Reconexão instantânea sem piscar a tela desnecessariamente
  - Driver não reinicia se pedir a mesma resolução

- 🛡️ Verificação de Permissões
  - Detecção automática se o programa é Administrador

### ⚙️ MENU DE CONFIGURAÇÕES DE STREAMING NO PC (NOVO):
- Detecção automática de Hardware e display de opções disponíveis
- Seleção manual de Codec: H.265, H.264, VP8
- Controle de Taxa de quadros: 30, 60, 90, 120 FPS
- Ajuste de Bitrate (Qualidade da imagem)
- Configurações avançadas com opções recomendadas aplicadas automaticamente
- Arquitetura multitarefa robusta: Serviços de rede e processamento rodam em threads independentes para evitar travamentos.

---

## 🎯 Casos de Uso

### 🕹️ Jogos PC Nativo
- Steam, Epic Games, Xbox Game Pass
- Controles Xbox/PlayStation nativos
- Motion controls em jogos suportados

### 🎮 Emuladores
- Cemu (Wii U): Motion controls perfeitos
- Yuzu/Ryujinx (Switch): Gyro aiming
- Dolphin (Wii): Controles de movimento
- PS2/PS3: Suporte via emulação

### 🎮 BARRA ACIMA DO TECLADO VIRTUAL COM AS TECLAS DE PC
- 🔤 **Teclas Extendidas Suportadas**
  - Inclui todas as teclas de função (F1 a F12)
  - Adiciona teclas de navegação: Page Up, Page Down, Home, End
  - Barra de exibição desse botões agora suporta rolagem para acessar todos os botões
  - Teclas Shift, Ctrl, Alt podem ser "travadas" em estado ativo
  - O indicador visual permanece destacado na interface até a desseleção manual (Botão fica Azul)

### 🖱️ USO DA TELA COMO TOUCHPAD PARA MOUSE
- 🎯 **Sistema de Clique Seguido por Hemisfério**
  - A tela de vídeo é dividida virtualmente em hemisfério esquerdo e direito
  - Toque longo no hemisfério esquerdo = clique esquerdo segurado
  - Toque longo no hemisfério direito = clique direito segurado
  - Liberação ocorre ao soltar o toque na respectiva área
  - Interface mostra indicadores visuais de click segurado
  - Divisão baseada na resolução nativa detectada automaticamente
  - Ponto central da tela (X/2) define a fronteira entre hemisférios

---

## 🔧 Arquitetura Técnica

| Recurso | Tecnologia | Status |
|---------|------------|---------|
| Controle | ViGEmBus (Kernel) | ✅ Pronto |
| Vídeo | GStreamer + NVENC/AMF + WebRTC (Aceleração por Hardware) | ✅ Pronto |
| Áudio | WASAPI Loopback + Roteamento UDP Dedicado + Reprodutor Nativo Kotlin | ✅ Pronto |
| Rede | TCP/UDP + Broadcast Discovery + Heartbeat | ✅ Pronto |
| Sensores | Protocolo Cemuhook UDP | ✅ Pronto |
| Segundo Plano Android | Serviço de Primeiro Plano com Notificação Persistente | ✅ Pronto |
| Monitor Virtual | Windows Display Driver API + PowerShell Automation | ✅ Pronto |
| Bluetooth | RFCOMM / BLE GATT | 🚧 Em Desenvolvimento(Ideia abandonada por enquanto, devido ao baixo suporte do windows a configs de bluetooth) |

---

## ⚡ Performance

- ⚡ Latência de controle: <8ms (125Hz)
- 🎬 Streaming: Até 60 FPS com baixo delay e sincronia áudio/vídeo aprimorada
- 🔊 Áudio: Qualidade Hi-Fi, estéreo real, sem compressão degradante (modo "aplicativo de música")
- 📊 Sensores: 100Hz sampling rate
- 🎯 Precisão analógica: 16-bit resolution
- 🖥️ Monitor Virtual: Aplicação instantânea de resoluções customizadas

---

## 🛠️ Configuração Recomendada

### 💻 PC
- Windows 10/11 64-bit
- GPU com encoder hardware (NVENC/AMF) recomendada para melhor performance
- 4GB RAM mínimo
- Conexão Wi-Fi 5GHz ou USB Tethering para melhor estabilidade
- Permissões de Administrador necessárias para configurar o Monitor Virtual

### 📱 Android
- Android 8.0+
- Giroscópio (recomendado para motion controls)
- Wi-Fi 5GHz ou USB Tethering
- 2GB RAM mínimo

---

## ❓ Suporte e Solução de Problemas

### 💻 Stream do monitor errado ou não carregada
1. Feche e abra o programa do PC e tente novamente (geralmente ele funciona de primeira)

### 🔍 Conexão Não Estabelecida
1. Verifique se estão na mesma rede Wi-Fi
2. Confirme que o firewall permite o aplicativo
3. Tente usar ancoragem USB via cabo

### 🎮 Controles Não Funcionam
1. Verifique a instalação do ViGEmBus (instalador na pasta \drivers\)
2. Confirme se o VC++ Redist está instalado
3. Teste com modo Xbox 360 primeiro

### 📹 Streaming com Lag ou Problemas
1. Use Wi-Fi 5GHz ou cabo USB
2. No menu de configurações do PC, reduza a taxa de quadros ou bitrate se necessário
3. Verifique se a aceleração por hardware (NVENC/AMF) está funcionando nas configurações
4. Ajuste o modo de visualização no app para "Split" se a conexão for mais lenta

### 🖥️ Problemas com Monitor Virtual
1. Permissões de Administrador: Execute o programa como Administrador (Botão direito → Executar como administrador)
2. Driver não instalado: Instale o Virtual Display Driver conforme instruções na seção de instalação
3. Tela não aparece: Aguarde 3-5 segundos após conexão para o Windows detectar o novo monitor
4. Resolução errada: Use o Modo Galera (1080p fixo) como fallback

### 🎯 Motion Controls em Emuladores
1. No programa do PC, verifique se o Servidor DSU está ativo
2. Configure o emulador para conectar em 127.0.0.1:26760
   - No Cemu: Input → Motion → DSU Client
   - No Yuzu: Configurações → Controles → Motion

### 🔊 Problemas de Áudio
1. Som "metálico" ou cortado: Isso foi resolvido. Certifique-se de usar a versão mais recente do App e Servidor.
2. Sem áudio no fone Bluetooth: Verifique se o fone está conectado ao celular antes de iniciar o streaming. O sistema detecta automaticamente na conexão.
3. Áudio cortando em 30 FPS: Corrigido com buffer otimizado. Se persistir, tente 60 FPS nas configurações do PC.

---

## 🚧 Funcionalidades Experimentais

### 📶 Bluetooth (Em Desenvolvimento)
- Conexão direta PC↔Celular via Bluetooth
- Menor consumo de bateria
- Largura de banda reduzida vs Wi-Fi

Nota: O Bluetooth está em fase de testes e pode não oferecer a mesma estabilidade que Wi-Fi/USB.

---

## 📄 LICENÇA E TERMOS DE USO

### 🔒 SOFTWARE PROPRIETÁRIO
- Código fonte fechado - não disponível publicamente
- Distribuição apenas do executável para uso final
- Modificações proibidas - não é permitida engenharia reversa

### 📝 TERMOS DE USO
- Uso gratuito para fins pessoais
- Proibida redistribuição sem autorização
- Não-comercial - uso pessoal apenas

### ⚠️ COMPONENTES DE TERCEIROS
Este software utiliza componentes de código aberto:
- ViGEmBus - Licença MIT (https://github.com/ViGEm/ViGEmBus)
- GStreamer - Licença LGPL (https://gstreamer.freedesktop.org)
- Virtual Display Driver - Licença MIT (https://github.com/VirtualDrivers/Virtual-Display-Driver)

### 🔐 DIREITOS AUTORAIS
O código original e implementações específicas são propriedade do desenvolvedor.

---

Transforme sua experiência de jogo com controle preciso, streaming de vídeo de alta performance e áudio de qualidade profissional! 🎬🎮🔊

Precisa de ajuda? Consulte a seção de solução de problemas acima ou abra uma issue no nosso GitHub!



