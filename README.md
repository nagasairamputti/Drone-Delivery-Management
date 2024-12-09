# My Drone Project

## Problem Statement

The final leg of the supply chain—known as last-mile delivery—accounts for up to 30% of total supply chain costs. It is also one of the most labor-intensive and time-consuming parts of the delivery process. The next evolution in delivery services is drone-based delivery. However, a major challenge is the efficient routing and distribution of delivery tasks across a fleet of drones.

## Solution

Our solution is an automated Delivery Management System that reduces overall delivery costs and optimizes battery usage. We leverage the **Capacitated Vehicle Routing Problem (CVRP)**, combined with **Genetic Algorithms**, to calculate the most efficient routes for drone deliveries. The CVRP addresses the need for vehicles (drones) with limited capacity to deliver items across various locations.

Special attention is given to **Emergency Deliveries** and **Prime Customers**, ensuring priority handling. Additionally, real-time drone tracking is integrated with Google Maps for efficient monitoring.

## Novelty

- **AI-Optimized Routing**: We use Artificial Intelligence to determine the most efficient delivery routes for drones.
- **Multi-Objective Optimization**: Non-dominated Sorting Genetic Algorithm II (NSGA-II) is used for optimizing multiple objectives, such as minimizing the number of drones required and reducing overall costs.
- **Multi-Packet Deliveries**: We manage constraints such as payload capacity and drone battery limits when delivering multiple packages.
- **Optimized Battery Consumption**: We use an improved version of the D'Andrea equation to accurately model battery consumption, considering factors like payload, air resistance, battery life cycle, and energy costs.

## Results

**Simulation**: The system has been tested with real-world scenarios to demonstrate its effectiveness in routing, delivery optimization, and battery management.






# Running the Project

To run the project on your local machine, follow these steps:

### 1. Install dependencies:
pip install -r requirements.txt

### 2. Run migrations:
cd dronehackon

python manage.py makemigrations

python manage.py migrate

### 3. Create a superuser:
python manage.py createsuperuser


### 4. Start the local development server:
python manage.py runserver

