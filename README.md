# Payment Gesture Simulation

Gesture recognition and trajectory tracking for simulated payment interactions.

## Summary
This repository contains Python code to simulate and record payment gestures in different scenarios (standing, sitting) and to run a TensorFlow Lite (TFL) agent for inference. It includes agents for different contexts and orchestration scripts to run experiments and record trajectories.

## Features
- Simulate payment gestures for standing and sitting scenarios
- TensorFlow Lite inference support
- Orchestrator to run end-to-end simulations
- Scripts to run, record, and export gesture data

## Repository layout
- agents/
  - PaymentAgent.py — base logic for payment gesture processing
  - PaymentStandingAgent.py — standing scenario agent
  - PaymentSittingAgent.py — sitting scenario agent
  - TFLAgent.py — TensorFlow Lite inference wrapper
  - Orchestrator.py — orchestration for running scenarios and collecting data
- scripts/
  - payment_standing_simulation_script.py
  - payment_sitting_simulation_script.py
  - tfl_simulation_script.py
  - orchestration_script.py
- README.md
- requirements.txt
- setup.py

## Requirements
- Python 3.8+
- Core Motion framework (for iOS data capture, optional for simulation)
- See requirements.txt for Python dependencies

## Installation
1. Clone the repo:
   ```bash
   git clone https://github.com/sandyphotographyuk-svg/PaymentGestureSimulation.git
   cd PaymentGestureSimulation
   ```
2. Create and activate a virtual environment:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate    # macOS / Linux
   .venv\Scripts\activate       # Windows (PowerShell)
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage examples
- Run the standing simulation:
  ```bash
  python scripts/payment_standing_simulation_script.py
  ```
- Run the sitting simulation:
  ```bash
  python scripts/payment_sitting_simulation_script.py
  ```
- Run TFL inference:
  ```bash
  python scripts/tfl_simulation_script.py --model path/to/model.tflite
  ```
- Run the orchestrator to run a sequence of scenarios:
  ```bash
  python scripts/orchestration_script.py
  ```

(Each script may accept additional CLI arguments — open the scripts to see available options.)

## Development
- Run linters / formatters as configured (add config as needed).
- Add unit tests under a tests/ directory.
- To package:
  ```bash
  python setup.py sdist bdist_wheel
  ```

## Contributing
Contributions welcome — open issues or PRs. Suggested contribution steps:
1. Fork the repo
2. Create a feature branch
3. Add tests for new behavior
4. Open a PR referencing the issue

## License
Suggest adding a license file (e.g., MIT). If you want, I can add a LICENSE file for you.

## Contact
Maintainer: sandyphotographyuk-svg
