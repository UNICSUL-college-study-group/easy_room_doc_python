# Projeto de Arquitetura

## Arquitetura em Camadas

1. **Front-end (React)**
   - **Componentes** para UI (ex: `HotelCard`, `BookingForm`).
   - **Rotas** com React Router.
   - **State Management** com Redux ou Context API.
   - **Consumo de APIs** com Axios.

2. **Back-end (Python)**
   - **Endpoints RESTful**:
     - `/api/hotels` – Listar hotéis.
     - `/api/bookings` – Criar/modificar reservas.
     - `/api/auth` – Autenticação.
   - **Modelos** com SQLAlchemy.
   - **Middleware** para validações e autenticação.

3. **Banco de Dados**
   - **Tabelas**:
     - `Users`: clientes e administradores.
     - `Hotels`: detalhes dos hotéis.
     - `Rooms`: informações dos quartos.
     - `Bookings`: registros de reservas.

## Diagrama de Arquitetura

[React Front-end] <--> [Python API (Flask/Django)] <--> [Banco de Dados SQL]