# meal-planner
This is our sem project....!!

Smart Recipe & Meal Planner Application built with Spring Boot 3 and modern web technologies.

## 🍽️ Features

- **Recipe Management**: Browse, search, filter (by dietary preference, cuisine, meal type, prep time), and add custom recipes with ingredients, instructions, and nutritional macros.
- **Weekly Meal Planner**: Drag-and-drop or assign recipes across Monday through Sunday for Breakfast, Lunch, Dinner, and Snacks.
- **Dynamic Shopping List**: Automatically aggregates grocery ingredients from your scheduled meals for hassle-free shopping.
- **User Authentication**: Secure signup and login with OTP email verification (via Spring Mail / Gmail SMTP) and guest access support.
- **Responsive UI**: Apple-inspired minimalist design with dark/light themes and smooth micro-interactions.

---

## 🛠️ Tech Stack

- **Backend**: Java 17, Spring Boot 3.2.3 (Spring Web, Spring Data JPA, Spring Security, Spring Mail)
- **Database**: H2 Database (File-based: `./data/recipes`)
- **Frontend**: HTML5, Vanilla JavaScript, CSS3, Google Material Symbols
- **Build Tool**: Maven

---

## 🚀 Getting Started

### Prerequisites
- Java 17 or higher
- Maven 3.8+ (or your IDE's bundled Maven)

### Running Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/pankajbendre987-prog/meal-planner.git
   cd meal-planner
   ```

2. **Run with Maven:**
   ```bash
   mvn spring-boot:run
   ```

3. **Access the Application:**
   - Web App: [http://localhost:8080](http://localhost:8080)
   - H2 Console: [http://localhost:8080/h2-console](http://localhost:8080/h2-console) (JDBC URL: `jdbc:h2:file:./data/recipes`)

### Configuration (Optional)
To enable real email OTP delivery, set these environment variables before starting:
- `MAIL_USERNAME`: Your Gmail address
- `MAIL_PASSWORD`: Your Gmail App Password

If unset, EmailService runs in development mode and logs OTP codes directly to the console.
