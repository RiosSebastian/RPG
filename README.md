# 🌾 Granja

Juego 2D top-down hecho con **Godot 4.5** y **GDScript**. Controlas a un guerrero que explora un mapa isla y pelea contra enemigos con ataques dirigidos con el mouse.

> Proyecto en desarrollo: actualmente hay un mapa de prueba con un jugador y un enemigo.

## Características

- Movimiento en 8 direcciones con animaciones de idle y correr.
- Ataque direccional: el golpe apunta hacia donde está el mouse (clic izquierdo).
- Máquina de estados del jugador (`IDLE`, `RUN`, `ATTACK`, `DEAD`).
- Enemigos con puntos de vida, recepción de daño y efecto de muerte.
- Mapa construido con `TileMapLayer`: agua, espuma, terreno, mesetas, sombras, props y nubes.
- Orden de dibujado por eje Y (y-sort) para profundidad.

## Controles

| Acción | Control |
|--------|---------|
| Moverse | Acciones `up`, `down`, `left`, `right` (configuradas en el Input Map) |
| Atacar | Clic izquierdo del mouse |

## Requisitos

- [Godot 4.5](https://godotengine.org/download) (renderizador Mobile)

## Cómo ejecutarlo

1. Clona el repositorio:
```bash
   git clone https://github.com/TU_USUARIO/granja.git
```
2. Abre Godot y elige **Importar**, luego selecciona el archivo `project.godot`.
3. Presiona **F5** para jugar. La escena principal es `scanes/map/test_map.tscn`.

## Estructura del proyecto

```
granja/
├── aseet/          # Sprites y tilesets (terreno, decoraciones, personajes)
├── resources/      # Recursos compartidos
├── scanes/
│   ├── player/     # Jugador (escena y script)
│   ├── enemies/    # Enemigos (escena y script)
│   ├── effects/    # Efectos, como la animación de muerte
│   └── map/        # Mapas y escenas de nivel
└── project.godot
```

## Estadísticas configurables

Desde el inspector de Godot puedes ajustar:

- **Jugador:** `speed`, `attack_speed`, `attack_damege`
- **Enemigo:** `hitpoints`, `death_packed`

## Próximos pasos

- [ ] IA del enemigo (perseguir y atacar al jugador)
- [ ] Vida y muerte del jugador
- [ ] Más enemigos y mapas
- [ ] Interfaz (barra de vida)

## Créditos

- Arte: completa aquí el autor y la licencia del pack de assets que usas.

## Licencia

Define aquí la licencia (por ejemplo MIT).
