# InviSolar Configurator

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Java](https://img.shields.io/badge/Java-8+-orange?logo=java)](https://www.java.com/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-2.x-green?logo=spring)](https://spring.io/projects/spring-boot)
[![Maven](https://img.shields.io/badge/Maven-3.x-red?logo=apache-maven)](https://maven.apache.org/)

Interactive web-based configurator for solar panel installations, enabling users to customize and visualize their renewable energy setup in real-time.

Developed for **InviSolar** as part of a web development project focusing on responsive design and user-centric configuration tools.

## Overview

This full-stack application provides an intuitive interface for configuring solar panel installations based on user requirements. The responsive design ensures optimal experience across desktop, tablet, and mobile devices, while the Spring Boot backend handles configuration logic and data management.

## Features

- **Interactive Configuration**: Real-time customization of solar panel setups with immediate visual feedback
- **Responsive Design**: Seamless experience across all device sizes and screen resolutions
- **User-Friendly Interface**: Intuitive navigation and clear configuration options
- **Dynamic Calculations**: Automatic computation of installation requirements and specifications
- **Configuration Export**: Save and share solar panel configurations
- **Modern Architecture**: Clean separation between frontend presentation and backend logic

## Technology Stack

### Frontend
- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with responsive layouts
- **JavaScript**: Interactive functionality and dynamic content

### Backend
- **Java 8+**: Core application logic
- **Spring Boot**: Framework for rapid development and deployment
- **Maven**: Dependency management and build automation

## Project Structure

```
Responsive_Configurator_Website_for_InviSolar/
├── src/
│   ├── main/
│   │   ├── java/                    # Java source files
│   │   │   └── [packages]           # Application logic
│   │   └── resources/               # Static resources
│   │       ├── static/              # CSS, JS, images
│   │       └── templates/           # HTML templates
├── pom.xml                          # Maven configuration
├── .gitignore
├── LICENSE
└── README.md
```

## Getting Started

### Prerequisites

Ensure you have the following installed:
- **Java Development Kit (JDK)**: 8 or higher
- **Apache Maven**: 3.6 or higher
- **Web Browser**: Modern browser (Chrome, Firefox, Safari, Edge)

Verify installations:
```bash
java -version
mvn -version
```

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/Cantellos/Responsive_Configurator_Website_for_InviSolar.git
cd Responsive_Configurator_Website_for_InviSolar
```

2. **Build the project**
```bash
mvn clean install
```

3. **Run the application**
```bash
mvn spring-boot:run
```

4. **Access the configurator**

Open your browser and navigate to:
```
http://localhost:8080
```

The configurator interface will load automatically.

### Alternative: Run JAR directly

After building, you can run the generated JAR:
```bash
java -jar target/invisolar-configurator-1.0.jar
```

## Usage

1. **Launch the application** at `http://localhost:8080`
2. **Configure your setup**:
   - Select panel type and quantity
   - Define installation parameters
   - View real-time calculations
3. **Review configuration** summary
4. **Export or save** your configuration

## Configuration Options

The configurator allows customization of:
- Solar panel types and models
- Number of panels
- Installation area and layout
- System capacity requirements
- Additional components (inverters, batteries, etc.)

## Development

### Running in Development Mode

```bash
mvn spring-boot:run -Dspring-boot.run.profiles=dev
```

### Building for Production

```bash
mvn clean package -DskipTests
```

The production-ready JAR will be generated in the `target/` directory.

### Testing

Run unit and integration tests:
```bash
mvn test
```

## Deployment

### Local Deployment
The application runs on embedded Tomcat server (default port 8080).

### Production Deployment
1. Build production JAR: `mvn clean package`
2. Deploy JAR to server
3. Run with: `java -jar invisolar-configurator.jar`
4. Configure reverse proxy (nginx/Apache) if needed

### Environment Variables
Configure application properties via environment variables:
- `SERVER_PORT`: Application port (default: 8080)
- `SPRING_PROFILES_ACTIVE`: Active profile (dev/prod)

## Project Context

This project was developed for **InviSolar**, a company specializing in solar energy solutions, as part of a web development initiative. The focus was on creating a responsive, user-friendly tool that simplifies the solar panel configuration process while maintaining technical accuracy.

**Key objectives:**
- Demonstrate responsive web design principles
- Implement clean architecture with Spring Boot
- Create intuitive user experience for complex configurations
- Ensure cross-device compatibility

## Browser Compatibility

Tested and supported on:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Future Enhancements

Potential improvements and features:
- [ ] Real-time cost estimation
- [ ] 3D visualization of panel layouts
- [ ] Integration with mapping APIs for roof analysis
- [ ] Multi-language support
- [ ] Export to PDF functionality
- [ ] Save configurations to user accounts
- [ ] Admin panel for managing products

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit changes: `git commit -m "Add new feature"`
4. Push to branch: `git push origin feature/my-feature`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Developed for **InviSolar**
- Part of web development coursework focusing on responsive design and full-stack development
- Built with Spring Boot framework and modern web technologies

## Contact

For questions or feedback, visit the [GitHub repository](https://github.com/Cantellos/Responsive_Configurator_Website_for_InviSolar) or open an issue.
