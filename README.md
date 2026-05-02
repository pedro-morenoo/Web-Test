/* Variables de color: Azul mar y Dorado arena */
:root {
  --primary-blue: #005f73;
  --accent-gold: #ee9b00;
  --text-dark: #333;
  --bg-light: #f9f9f9;
}

/* Contenedor principal en Cuadrícula */
.menu-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 25px;
  padding: 20px;
  background-color: var(--bg-light);
}

/* La Tarjeta Modernizada */
.menu-card {
  background: white;
  border-radius: 15px;
  overflow: hidden;
  box-shadow: 0 10px 20px rgba(0,0,0,0.05);
  transition: transform 0.3s ease;
  display: flex;
  flex-direction: column;
}

.menu-card:hover {
  transform: translateY(-10px); /* Efecto de levitación */
}

/* Imagen con Badge */
.card-image {
  position: relative;
  height: 200px;
}

.card-image img {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Para que la foto no se deforme */
}

.badge {
  position: absolute;
  top: 10px;
  right: 10px;
  background: var(--accent-gold);
  color: white;
  padding: 5px 12px;
  border-radius: 20px;
  font-size: 0.8rem;
  font-weight: bold;
}

/* Contenido de la tarjeta */
.card-content {
  padding: 20px;
}

.card-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 10px;
}

.card-header h3 {
  margin: 0;
  color: var(--primary-blue);
  font-size: 1.3rem;
}

.price {
  font-weight: bold;
  color: var(--text-dark);
  font-size: 1.2rem;
}

.card-content p {
  font-size: 0.95rem;
  color: #666;
  line-height: 1.4;
}

/* Alérgenos discretos */
.card-footer {
  margin-top: 15px;
  border-top: 1px solid #eee;
  padding-top: 10px;
}

.allergen {
  font-size: 0.75rem;
  background: #eee;
  padding: 3px 8px;
  border-radius: 4px;
  margin-right: 5px;
}
