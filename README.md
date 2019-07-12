# Modo Competitivo 5v5 para Counter Strike 1.6

Tome lo mejor de varios plugins para hacerlo un poco mas automatico. Por ejemplo, inicia automaticamente al estar 10 jugadores en el servidor, kickea automaticamente a los AFK y muestra el daño que realizaste en una ronda justo luego de morir.

## Caracteristicas 
- Inicio de juego automatico
- Menu general en la tecla N
- Pausar el partido
- Mutear y desmutear
- Expulsar jugador de la partida
- DMG automatico en consola
- Empate disponible y configurable
- Mantiene puntuaciones al cambio de bando
- Los vivos pueden leer a los muertos

## Requisitos

- [Amxmodx 1.8.x](https://www.amxmodx.org/downloads.php)
- [Regamedll 5.x](https://github.com/s1lentq/ReGameDLL_CS)
- [Reapi 5.6.x](https://github.com/s1lentq/reapi)

## Comandos de chat

- Administrador<br>
	.start		- Forza el inicio del pug<br>
	.cancel		- Forza el final del pug<br>
	.manual		- El modo iniciara manualmente<br>
	.auto		- El modo iniciara automaticamente<br>

- Jugador<br>
	.menu				- Menu de funcionalidades (tecla N)<br>
	.votekick <nombre>	- Votacion para expulsar a un jugador<br>
	.votepause			- Votacion para pausar partido<br>
	.mute <nombre>		- Mutear jugador<br>
	.unmute <nombre>	- Desmutear jugador<br>

## Configuraciones destacables  (pugconfig.cfg)

| Cvar                 | Default    | Descripción |
| :------------------- | :--------: | :--------------------------------------------------- |
| pug_tag              | "[Server]" | Prefix del servidor                                  |
| pug_owner	           | ""         | Nombre de los lideres del servidor                   |
| pug_rounds_max       | 30         | Rondas maximas del partido                           |
| pug_rounds_ot        | 6          | Rondas maximas del overtime                          |
| pug_allow_tie        | 0          | Activa el empate de la partida                       |
| pug_show_money       | 1          | Muestra el dinero de los jugadores. <br/>`0` Deshabilitado<br/>`1` Por chat<br/>`2` Por HUD<br/>`3` Por sprites |
| pug_votepause_time   | 60         | Tiempo (seg) que duran las pausa                     |
| pug_afktime          | 60         | Tiempo (seg) en que sera kickeado un jugador por afk |

## Cosas por hacer
- Añadir ronda a cuchillo y configurar por cvar
- Que los espectadores entren automaticamente por orden de llegada
- Bloquear modo espectador, solo para admins
- Refactorizar todo el codigo por modulos (includes)

## Agradecimientos | Autores de otros pugmod 

[Sugisaki](https://amxmodx-es.com/Thread-Competitive-Face-it-Pick-Up-Game-PUG)<br>
[PredatorFlys](https://amxmodx-es.com/Thread-Auto-Mix-YAP-Capitan-resubido)<br>
[SmileYzn](https://github.com/SmileYzn/CS_PugMod)<br>

