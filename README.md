# Install de ComfyUI pour FLUX
basé sur le dossier CPC Hardware 65

## Pré requis

* Linux
* [UV](https://docs.astral.sh/uv/) et git
* carte nvidia

## Install

```git clone https://github.com/comfyanonymous/ComfyUI.git```

ensuite dans ComfyUI/custom_nodes

```git clone https://github.com/city96/ComfyUI-GGUF```


## Fichiers

Télécharger les fichiers suivants :

* https://cpc.cx/ModeleFlux
* https://cpc.cx/ModeleT5
* https://cpc.cx/ModeleVAE
* https://cpc.cx/ModeleCLIP

Placer les fichiers :

* flux1-dev-Q4_K_S.gguf dans ComfyUI/models/unet/
* clip_l.safetensors et t5xxl_fp8_e4m3fn.safetensors dans ComfyUI/models/text_encoders/
* flux_vae.safetensors dans ComfyUI/models/vae/

## Lancement

Pour lancer l'interface ComfyUI :

```uv run ComfyUI/main.py```

Ouvrir le fichier fluxcpc.json pour un exemple fonctionnel.