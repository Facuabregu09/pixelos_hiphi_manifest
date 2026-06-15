# PixelOS 16 (Android 16.2) - Local Manifest para Motorola Edge 30 Pro (hiphi)

Local manifest para compilar PixelOS 16.2 (rama sixteen-qpr2) en el
Motorola Edge 30 Pro (hiphi / XT2201-1 / SM8450).

## Uso

1. Inicializar el source de PixelOS:
   repo init -u https://github.com/PixelOS-AOSP/manifest.git -b sixteen-qpr2

2. Copiar hiphi.xml a .repo/local_manifests/:
   mkdir -p .repo/local_manifests
   cp hiphi.xml .repo/local_manifests/

3. Sincronizar:
   repo sync -c -j$(nproc)

4. Compilar:
   source build/envsetup.sh
   breakfast hiphi user
   m pixelos -j$(nproc)

## Creditos

- Device & vendor trees: ThE_MarD (motorola-sm8450-devs)
- Kernel con fix de recovery: Facuabregu09
- Mantenedor: Facundo Abregu
