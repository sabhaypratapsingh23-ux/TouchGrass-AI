# TrailSpark

TrailSpark turns a nearby place, a bit of free time, and a mood into a three-step outdoor micro-adventure. It is a plain HTML/CSS/JavaScript project; open-weight inference runs locally in the browser through the open-source [WebLLM](https://github.com/mlc-ai/web-llm) runtime and the Qwen2.5 1.5B Instruct model.

## Run it

1. Install Node.js 20 or newer.
2. In this folder, run `npm install`.
3. Run `npm run dev` and open the local URL Vite prints.
4. Use a recent WebGPU-capable Chrome or Edge browser. The first AI setup downloads model weights; later visits can reuse the browser cache.

## Open innovation

The planner uses an open-weight model and an open-source inference runtime. Once the model is cached, prompts and generated plans are processed on the device and no AI server receives them. You can replace the model ID in `app.js` with another model supported by WebLLM, or adjust the system prompt to change the guide's behavior. The first model download requires internet, storage, and a compatible browser/GPU.

The first screen is deliberately short: the result is a three-step prompt, and the final button encourages putting the phone away. It avoids claiming live trail, weather, or wildlife data.
