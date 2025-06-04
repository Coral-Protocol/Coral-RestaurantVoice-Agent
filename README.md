# Restaurant Voice Agent System

## Responsibility:
A multi-agent voice conversation system for restaurants that handles reservations, takeaway orders, and checkout through natural voice interactions. Features four specialized AI agents that seamlessly transfer conversations while maintaining context.

## Details
- **Framework:** LiveKit Agents
- **Tools Used:** Deepgram STT, Cartesia TTS, OpenAI LLM, Silero VAD
- **AI Model:** GPT-4
- **Date Added:** January 2025
- **License:** MIT
- **Original Source:** [Restaurant Voice Agent System](https://github.com/livekit/agents/blob/main/examples/voice_agents/restaurant_agent.py)

## Install Dependencies
```bash
pip install uv
uv sync
```

## Configure Environment Variables
Copy the example file and add your API keys:

```bash
cp env.example .env
```

Update `.env` with:
- `LIVEKIT_URL`
- `LIVEKIT_API_KEY`
- `LIVEKIT_API_SECRET`
- `OPENAI_API_KEY`
- `DEEPGRAM_API_KEY`
- `CARTESIA_API_KEY`

## Run Agent
```bash
uv run python main.py console
```

## Agent System

### 🏪 Greeter Agent
Restaurant receptionist that welcomes customers, presents menu (Pizza $10, Salad $5, Ice Cream $3, Coffee $2), and routes to specialized agents.

### 📅 Reservation Agent
Handles dining reservations - collects time, customer name, and phone number.

### 🥡 Takeaway Agent
Processes food orders - takes orders from menu, clarifies requests, confirms details.

### 💳 Checkout Agent
Handles payments - calculates expenses, collects contact info and credit card details.

## Usage Examples

**Making a Reservation:**
1. Say: "I'd like to make a reservation"
2. Provide preferred time, name, and phone
3. Confirm details

**Ordering Takeaway:**
1. Say: "I want to order food"
2. Place order from menu
3. Provide payment information
4. Complete transaction

## Creator Details
- **Name:** Ahsen Tahir
- **Contact:** ahsen.t@coralprotocol.org
