# Animefootball — MiniMax-H3 2D Anime Football Movement LoRA

A motion and domain-knowledge LoRA for **MiniMax-H3** designed to replace the base model's forced cinematic camera movement with authentic 2D anime football (soccer) body mechanics and ball physics.

Out of the box, MiniMax-H3 lacks awareness of technical football skills (such as rainbow flicks, sharp dribbling, and body feints) and defaults to generic cinematic motion. This LoRA teaches the model proper anime body posture, footwork, and dynamic 2D action flow.

## Download
Download `animefootball.safetensors` from the page and place it in the lora nod of ComfyUI setup with recommended strength of 0.6 or slightly higher.


## How to Use
- **Base Model:** MiniMax-H3 (Image-to-Video / Reference-to-Video)
- **Trigger Word:** `Animefootball`
- **Recommended LoRA Strength:** `0.6` – `0.8` *(adjust to your sweet spot)*
- **Required Input:** **Reference first frame image + text prompt.** This LoRA is built for Image-to-Video / Reference-to-Video generation and requires a clear starting scene frame to anchor the player and ball.

### Supported Football Concepts & Prompts
Include the trigger word `Animefootball` alongside specific football actions:
- `rainbow flick`
- `dribbling` / `ball control`
- `body feint`
- `power shot`
- `slide tackle`


## Training Details
- **Dataset:** 70 curated 2D anime football video clips
- **Clip Length:** 24 to 34 frames per clip
- **Captioning:** Manually/detailed action-captioned focusing on football terminology, body mechanics, and 2D anime motion

## Limitations
- Designed specifically for **Image-to-Video / Reference-to-Video** workflows; results without a reference starting frame will be inconsistent.
- Works best on 2D anime character art styles rather than photorealistic footage.