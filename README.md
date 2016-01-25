## Slug Codes

| Code | Message                         | Type
-------|---------------------------------|--------------
|  1   | ServerStateMessage              | Shared
|  2   | ServerWorldStateMessage         | Shared
|  5   | ServerCommunicationMessage      | Communication
| 20   | SlugConfigureChassisRequest     | Configure
| 22   | SlugConfigureCockpitRequest     | Configure
| 24   | SlugConfigureTorsoRequest       | Configure
| 26   | SlugConfigureArmsRequest        | Configure
| 28   | SlugConfigureLegsRequest        | Configure
| 30   | SlugConfigureDoneRequest        | Configure
| 50   | SlugQueryMechRequest            | Query
| 51   | SlugQueryMechReponse            | Query
| 60   | SlugCommitCounterMeasureMessage | Commit
| 62   | SlugCommitWeaponRequest         | Commit
| 64   | SlugCommitMechRequest           | Commit
| 66   | SlugCommitCommunicationRequest  | Commit
| 68   | SlugCommitComputerRequest       | Commit
| 70   | SlugCommitSensorRequest         | Commit
| 72   | SlugCommitEngineRequest         | Commit
| 74   | SlugCommitActuatorRequest       | Commit
| 101  | ServerSlugGenericResponse       | Generic
| 102  | SlugActionLoginRequest          | Command
| 103  | SlugActionLoginResponse         | Command

## Server State Codes

| Code | State
-------|-----------------------------
| 1    | Initializing
| 2    | WaitingForSlugs
| 3    | Ready

## World State Codes

| Code | State
-------|-----------------------------
| 1    | Initializing
| 2    | ConfigurationPhase
| 3    | StartupPhase
| 4    | GamePhase
| 5    | GameOverPhase

## Error Codes

### State Error Codes

| Code | Error                       
-------|-----------
| 50   | WrongState

### Configuration Error Codes

| Code | Error                       
-------|-----------------------------
| 100  | ActuatorNotFound Model
| 101  | AmmoNotFound Model
| 102  | ArmNotFound Model
| 103  | ArmNoIndex ComponentId
| 104  | ArmNotConfigured
| 105  | ArmorNotFound Model
| 106  | CapacitorNotFound Model
| 107  | ChassisNotFound Model
| 108  | ChassisNotConfigured
| 109  | CockpitNotFound Model
| 110  | CockpitNotConfigured
| 111  | CommunicationNotFound Model
| 112  | CommunicationsOverLimit
| 113  | ComputerNotFound Model
| 114  | ComputersOverLimit
| 115  | CounterMeasureNotFound Model
| 116  | CounterMeasureOverLimit
| 117  | EngineNotFound Model
| 118  | GyroNotFound Model
| 119  | LegNotFound Model
| 120  | LegNoIndex ComponentId
| 121  | LegNotConfigured
| 122  | OverChassisMaxWeight
| 123  | ProtocolMismatch
| 124  | ReactorNotFound Model
| 125  | SensorNotFound Model
| 126  | SensorOverLimit
| 127  | TorsoNotFound Model
| 128  | TorsoNotConfigured
| 129  | WeaponNotFound Model
| 130  | WeaponOverLimit

## Simulation Codes

These are sent from the server to the 3d client.

| Code | Message                          | Type
-------|----------------------------------|------------
|    1 | ServerStateMessage               | Shared
|    2 | ServerWorldStateMessage          | Shared
|    5 | ServerClientObjectSpawnMessage   | Simulation
|    6 | ServerClientObjectMoveMessage    | Simulation
|    7 | ServerClientObjectDestroyMessage | Simulation
|  200 | ClientActionLoginRequest         | Command
|  201 | ClientActionLoginResponse        | Command

### Object Type Codes

| Code | Type
-------|------------
| 1    | Mech1
| 100  | Projectile1
| 120  | Missile1
| 140  | Rocket1
| 160  | Mortar1
| 180  | Beam1
| 200  | Explosion1
| 250  | Destroyed1
| 251  | Despawned1
