# Atlas Zero

Pacote ROS 2 para simulação de um robô quadrado em Gazebo.

## Sobre

`atlas-zero` é um pacote ROS 2 que define e simula um robô com formato quadrado (chassis) movido por quatro rodas, utilizando o simulador Gazebo. O projeto utiliza URDF/Xacro para descrever a geometria do robô e inclui configurações para simulação física em ambiente controlado.

## Tecnologias

- **ROS 2** (Robot Operating System)
- **Gazebo** - Simulador de robótica
- **URDF/Xacro** - Descrição de robôs
- **ament_cmake** - Build system para ROS 2

## Estrutura

```
atlas-zero/
├── launch/           # Arquivos de lançamento (launch files)
│   ├── rsp.launch.py       # Lançamento do robot_state_publisher
│   └── launch_sim.launch.py # Lançamento completo com Gazebo
├── description/       # Descrição do robô em Xacro/URDF
├── worlds/           # Mundos Gazebo (SDF)
├── config/           # Configurações do projeto
└── CMakeLists.txt    # Arquivos de build
```

## Uso

Para iniciar a simulação:

```bash
ros2 launch atlas-zero launch_sim.launch.py
```

O robô será espalhado no mundo Gazebo usando o arquivo `robot.urdf.xacro` como descrição.
