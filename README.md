# 🎧 Dolby Atmos Preset para Easy Effects

Este preset proporciona una experiencia de audio envolvente y optimizada para Linux, diseñado específicamente para mejorar la profundidad y el escenario sonoro en altavoces.

> [!IMPORTANT]
> **Easy Effects requiere PipeWire** como servidor de sonido. Si utilizas versiones antiguas de Ubuntu o Mint que aún usan PulseAudio, podrías experimentar problemas de compatibilidad.

---

## 🚀 Guía de Instalación de Easy Effects

Dependiendo de tu distribución, utiliza los siguientes comandos:

### 1. Ubuntu y Linux Mint
Para versiones recientes (Ubuntu 22.04+ o Mint 21+):

* **Instalación estándar:**
    ```bash
    sudo apt update && sudo apt install easyeffects
    ```

* **Vía PPA (Recomendado para tener la última versión):**
    ```bash
    sudo add-apt-repository ppa:wwmm/easyeffects
    sudo apt update
    sudo apt install easyeffects
    ```

### 2. Arch Linux y Manjaro
En distribuciones basadas en Arch, el paquete suele estar siempre actualizado:

* **Instalación con Pacman:**
    ```bash
    sudo pacman -S easyeffects
    ```

* **Versión de desarrollo (AUR):**
    ```bash
    yay -S easyeffects-git
    ```

### 3. Método Universal (Flatpak) - ⭐ Recomendado
Es la forma más segura ya que incluye todas las dependencias necesarias.

1.  **Instalar Flatpak** (si no lo tienes):
    * Ubuntu/Mint: `sudo apt install flatpak`
    * Arch/Manjaro: `sudo pacman -S flatpak`
2.  **Instalar Easy Effects:**
    ```bash
    flatpak install flathub com.github.wwmm.easyeffects
    ```

---

## ⚠️ Nota importante sobre PipeWire

Si tras la instalación el programa no abre o no detecta el servidor de sonido, activa PipeWire manualmente (en Ubuntu/Mint):

```bash
sudo apt install pipewire-audio-client-libraries libspa-0.2-bluetooth libspa-0.2-jack
systemctl --user --now enable pipewire pipewire-pulse wireplumber
  ```

## 🛠️ Cómo aplicar este Preset

Sigue estos pasos para cargar la configuración en tu sistema:

1. **Descargar el archivo**: Baja el archivo `.json` que se encuentra en este repositorio.
2. **Abrir la aplicación**: Inicia **Easy Effects** desde tu menú de aplicaciones.
3. **Acceder a Presets**: Haz clic en el botón **Presets** ubicado en la esquina superior izquierda de la ventana.
4. **Importar**: Haz clic en el botón **Importar** (icono de carpeta o botón de texto según tu versión) y selecciona el archivo `.json` que descargaste.
5. **Cargar el Preset**: 
   - Busca **"Dolby Atmos"** en la lista de presets disponibles.
   - Haz clic en el **icono de la flecha hacia la derecha** (Cargar/Load) para activar todos los efectos automáticamente.

> [!TIP]
> Puedes marcar la casilla **Default** (Predeterminado) al lado del nombre del preset para que se aplique automáticamente cada vez que inicies sesión.
