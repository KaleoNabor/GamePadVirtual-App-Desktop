# 🎮 GamePadVirtual - Controle Universal com Streaming

Transforme seu smartphone Android em um controle profissional para PC com streaming de áudio e vídeo de baixa latência.

---

## 📦 **Downloads**

### 📱 Aplicativo Android
**Versão:** 1.3.0  
**Plataforma:** Android 8.0+  
**Arquivo:** `GamePadVirtual-Android-v-.-.-.apk`  
[📥 Baixar APK](https://github.com/KaleoNabor/GamePadVirtual-App-Desktop/releases/tag/App)

### 🖥️ Servidor PC
**Versão:** 1.3.0  
**Plataforma:** Windows 10/11 (64-bit)  
**Arquivo:** `GamePadVirtual-Server-v-.-.-.zip`  
[📥 Baixar Servidor](https://github.com/KaleoNabor/GamePadVirtual-App-Desktop/releases/tag/Server)

---

## 🚀 **Funcionalidades Principais**

### 🎯 **Controle Universal Multi-Plataforma**
- **Emulação Xbox 360 & DualShock 4** via ViGEmBus
- **Reconhecimento nativo** pelo Windows e jogos
- **Suporte a controles físicos** via Bluetooth/OTG
- **Multitouch** com até 8 toques simultâneos

### 🖥️ **Streaming de Vídeo & Áudio**
- **Captura direta da tela** via DirectX 11 (Zero-Copy)
- **Codificação hardware** NVENC (NVIDIA) / AMF (AMD)
- **Áudio do sistema** em tempo real via WASAPI
- **Latência ultrabaixa** com WebRTC

### 📡 **Conexão Híbrida**
- **Wi-Fi automático** com descoberta de rede
- **Ancoragem USB** para máxima estabilidade
- **TCP/UDP otimizado** para dados e vídeo
- **Reconexão automática** se a conexão cair

### 🎮 **Motion Controls para Emuladores**
- **Servidor DSU** nativo (porta 26760)
- **Compatibilidade total** com Cemu, Yuzu, Ryujinx, Dolphin(Somente por controle de PS4)
- **Giroscópio e acelerômetro** de alta precisão
- **Mira por movimento** em jogos compatíveis

### 🛠️ **Ferramentas Avançadas**
- **Editor de layout** arrastar-e-soltar
- **Touchpad** para controle do mouse
- **Teclado virtual** completo
- **Vibração háptica** local e remota

---

## ⚙️ **Instalação Rápida**

### 🔵 **Pré-requisito Obrigatório (PC)**
**Visual C++ Redistributable 2015-2022**  
📥 [Download Direto Microsoft](https://aka.ms/vs/17/release/vc_redist.x64.exe)

### 📋 **Passo a Passo**
1. **🔵 Instale o VC++ Redist** no PC (como Administrador)
2. **📥 Baixe o servidor** e extraia o ZIP
3. **🖥️ Execute** `GamePadVirtual-Desktop.exe`
4. **✅ Permita** a instalação do driver ViGEmBus
5. **📱 Instale o app** no celular
6. **🔍 Conecte** via "Descoberta Automática"
7. **🎮 Pronto para jogar!**

---

## 🎯 **Casos de Uso**

### 🕹️ **Jogos PC Nativo**
- **Steam, Epic Games, Xbox Game Pass**
- **Controles Xbox/PlayStation** nativos
- **Motion controls** em jogos suportados

### 🎮 **Emuladores**
- **Cemu (Wii U):** Motion controls perfeitos
- **Yuzu/Ryujinx (Switch):** Gyro aiming
- **Dolphin (Wii):** Controles de movimento
- **PS2/PS3:** Suporte via emulação

### 💻 **Controle do PC**
- **Touchpad** para mouse
- **Teclado virtual** para digitação
- **Atalhos rápidos** (Win, Alt+Tab, Esc)

---

## 🔧 **Arquitetura Técnica**

| Recurso | Tecnologia | Status |
|---------|------------|---------|
| **Controle** | ViGEmBus (Kernel) | ✅ **Pronto** |
| **Vídeo** | GStreamer + NVENC/AMF + WebRTC | ✅ **Pronto** |
| **Áudio** | WASAPI Loopback + Opus | ✅ **Pronto** |
| **Rede** | TCP/UDP + Broadcast Discovery | ✅ **Pronto** |
| **Sensores** | Protocolo Cemuhook UDP | ✅ **Pronto** |
| **Bluetooth** | RFCOMM / BLE GATT | 🚧 **Em Desenvolvimento** |

---

## ⚡ **Performance**

- **⚡ Latência de controle:** <8ms (125Hz)
- **🎬 Streaming:** 60 FPS com baixo delay
- **📊 Sensores:** 100Hz sampling rate
- **🎯 Precisão analógica:** 16-bit resolution
- **🔊 Áudio:** 128kbps Opus (low-delay)

---

## 🛠️ **Configuração Recomendada**

### 💻 **PC**
- Windows 10/11 64-bit
- GPU com encoder hardware (NVENC/AMF)
- 4GB RAM mínimo
- Conexão Wi-Fi 5GHz ou USB Tethering

### 📱 **Android**
- Android 8.0+
- Giroscópio (recomendado)
- Wi-Fi 5GHz ou USB Tethering
- 2GB RAM mínimo

---

## ❓ **Suporte e Solução de Problemas**

### 🔍 **Conexão Não Estabelecida**
1. Verifique se estão na mesma rede Wi-Fi
2. Confirme que o firewall permite o aplicativo
3. Tente usar ancoragem USB via cabo

### 🎮 **Controles Não Funcionam**
1. Verifique a instalação do ViGEmBus
2. Confirme se o VC++ Redist está instalado
3. Teste com modo Xbox 360 primeiro

### 📹 **Streaming com Lag**
1. Use Wi-Fi 5GHz ou cabo USB
2. Reduza a qualidade no app se necessário
3. Verifique encoder hardware na GPU

### 🎯 **Motion Controls em Emuladores**
1. Configure o emulador para conectar em `127.0.0.1:26760`
2. No Cemu: Input → Motion → DSU Client
3. No Yuzu: Configurações → Controles → Motion

---

## 🚧 **Funcionalidades Experimentais**

### 📶 **Bluetooth (Em Desenvolvimento)**
- **Conexão direta** PC↔Celular via Bluetooth
- **Menor consumo** de bateria
- **Largura de banda** reduzida vs Wi-Fi

*Nota: O Bluetooth está em fase de testes e pode não oferecer a mesma estabilidade que Wi-Fi/USB.*

---

## 📄 **Licença e Termos**

- **Licença:** MIT
- **Uso livre** para fins pessoais
- **Código aberto** disponível no GitHub
- **Sem garantias** - use por sua conta e risco

---

**Transforme sua experiência de jogo com controle preciso e streaming profissional!** 🎬🎮

*Precisa de ajuda? Abra uma issue no nosso GitHub!*

