# Open School Management Platform  
An open-source platform for managing school operations.

**Status**: *Planning Phase*

---

### Prototype Tech Stack:
- **Flask**: Lightweight Python web framework  
- **HTMX**: Enables dynamic page updates  
- **SQLite**: Simple and efficient database solution  
- **Pandas**: Powerful data manipulation and analysis library  
- **Bootstrap**: Frontend UI framework  
- **Popper.js**: Positioning library for tooltips and popovers  

#### Motivation:  
The goal is to quickly prototype a functional school management platform using a Python-based tech stack. Flask is chosen for its simplicity and rapid development capabilities, providing an ideal foundation for the initial prototype.

---

### Production Tech Stack:
- **Fiber**: High-performance web framework (replacing Flask)  
- **HTMX**: Dynamic page updates (remains the same as prototype)  
- **SQLite**: Lightweight database solution (same as prototype)  
- **Gota**: Data manipulation and analysis (replacing Pandas)  
- **Bootstrap**: Frontend UI framework (same as prototype)  
- **Floating UI**: Advanced positioning for popovers and tooltips (replacing Popper.js)  

#### Motivation:  
While Flask is excellent for rapid prototyping, it has certain scalability limitations that may pose challenges in a production environment. Fiber is chosen to overcome these bottlenecks and provide better performance. Gota will take over the data manipulation tasks previously handled by Pandas, and Floating UI will replace Popper.js as the recommended successor for handling advanced positioning of popovers and tooltips.

---

### Runtime Benchmark by World Wide Technology

|           | Peak CPU Usage % | Peak Memory Usage MB | 1. Requests/sec | 2. Requests/sec | 3. Requests/sec |
|-----------|------------------|----------------------|-----------------|-----------------|-----------------|
| Bun       | 25               | 207                  | 743             | 1679            | 1670            |
| C#        | 33               | 46                   | 747             | 1409            | 1277            |
| Go        | 28               | 22                   | 913             | 1635            | 1588            |
| Node.js   | 44               | 67                   | 374             | 1110            | 903             |
| Python    | 62               | 46                   | 221             | 406             | 378             |

While this benchmark is limited in scope, it aligns with broader and more detailed benchmarks that indicate Python, and by extension Flask, tends to underperform compared to other alternatives. This performance gap is a key reason for migrating from Flask in the production release.

*Source: [World Wide Technology Benchmark Report](https://www.wwt.com/blog/performance-benchmarking-bun-vs-c-vs-go-vs-nodejs-vs-python)*

---

### Version Roadmap

**Alpha Stage**
- **0.1**: Basic operational web application with core functionality and database integration  
- **0.2**: Admin interface for managing elevated user roles  
- **0.3**: User dashboard and profile page  
- **0.4**: Features for class schedule generation, attendance tracking, grade management, homework tracker and more
- **0.5**: Direct messaging between users, message groups and more
- **0.6**: Enhanced reporting and analytics
- **0.7**: Parent and guardian portal
- **0.8**: Integration with third-party tools and services

**Beta Stage**
- **0.9**: Prototype release with comprehensive testing, performance optimization, and user feedback implementation

**Production Release**
- **1.0**: Full production release

---
