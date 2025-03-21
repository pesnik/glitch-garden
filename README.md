# Glitch Garden

![Glitch Garden Logo](https://via.placeholder.com/150x150)

> **Turning chaos into wisdom: Master distributed systems through interactive simulation**

## Overview

Glitch Garden is an innovative simulation platform that helps engineers, developers, and organizations learn distributed system concepts through hands-on, interactive experiences. By safely simulating real-world failure scenarios in a controlled environment, users can visualize complex distributed system behaviors, understand common fallacies, and develop effective resilience strategies.

## Key Features

- 🔄 **Dynamic Simulation Orchestration**: Configure and deploy containerized distributed system nodes through an intuitive web dashboard
- 🧪 **Controlled Chaos**: Inject failures such as network partitions, latency, and node crashes to test system resilience
- 📊 **Real-time Visualization**: Watch how your distributed system responds to failures with live status updates and performance metrics
- 🎓 **Guided Learning**: Follow structured modules covering essential distributed systems concepts and fallacies
- 📝 **Comprehensive Analytics**: Generate detailed reports on system behavior during chaos experiments

## Getting Started

### Prerequisites

- Docker and Docker Compose
- Node.js (v14+)
- Rust toolchain (for simulation engine)
- MongoDB (local or cloud instance)

### Quick Start

```bash
# Clone the repository
git clone https://github.com/pesnik/glitch-garden.git
cd glitch-garden

# Install dependencies
npm install

# Start the MongoDB service (if running locally)
docker-compose up -d mongodb

# Start the simulation engine
cd simulation-engine && cargo run --release

# Start the web application
npm run dev
```

Then navigate to `http://localhost:3000` to access the dashboard.

## Architecture

Glitch Garden consists of four main components:

1. **Web Dashboard**: React.js frontend for simulation configuration and visualization
2. **API Server**: Golang (or Node.js) backend for orchestration and user management
3. **Simulation Engine**: Rust with MadSim for deterministic simulation execution
4. **Garden Nodes**: Docker containers representing distributed system components

![Architecture Diagram](https://via.placeholder.com/600x300)

## Use Cases

- **Learning**: Master distributed system concepts through hands-on simulation
- **Testing**: Verify system resilience against common failure modes
- **Training**: Upskill engineering teams in distributed systems principles
- **Experimentation**: Explore new patterns and strategies for system reliability

## Contributing

We welcome contributions to Glitch Garden! Please check our [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## Development Roadmap

### Current MVP (4-6 weeks)

- [x] Project setup and infrastructure
- [ ] Basic simulation orchestration
- [ ] Containerized distributed nodes
- [ ] Simple failure injection mechanisms
- [ ] Real-time monitoring dashboard
- [ ] Introductory learning modules

### Future Enhancements

- Advanced failure scenarios (Byzantine faults, split-brain)
- Custom simulation scripting
- Collaborative workspaces
- Public simulation sharing
- Integration with monitoring tools
- Advanced analytics and recommendations

## License

Glitch Garden is licensed under the [MIT License](LICENSE).

## Contact

For questions, feedback, or support, please [open an issue](https://github.com/pesnik/glitch-garden/issues) or contact the team at support@glitchgarden.io.

---

*"Perfection is finally attained not when there is no longer anything to add, but when there is no longer anything to take away." — Antoine de Saint-Exupéry*
