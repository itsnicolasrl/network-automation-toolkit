# Network Automation Toolkit

Conjunto de scripts para automatizar tareas repetitivas de administración de red: backups, cambios masivos y auditorías.

## 🎯 Objetivo
Eliminar la configuración manual dispositivo por dispositivo, reducir errores humanos y dejar trazabilidad de cambios.

## 🛠️ Stack
- Python 3.x
- Netmiko / Nornir
- [Librerías adicionales: netaddr, PyYAML, etc.]

## 📂 Estructura

├── inventory/ # inventario de dispositivos (Nornir) 
├── scripts/ 
├── backup_configs.py  
├── audit_ports.py 
│     └── bulk_vlan_change.py 
            └── logs/

## ⚙️ Funcionalidades
- **Backup automático de configs:** [cómo se ejecuta, cada cuánto, dónde se guarda]
- **Auditoría de puertos:** [qué revisa: puertos sin uso, VLANs mal asignadas, etc.]
- **Cambios masivos de VLAN:** [cómo se define el cambio, a qué dispositivos aplica]

## 🚀 Uso
```bash
python scripts/backup_configs.py --inventory inventory/devices.yaml
```

## 🔒 Seguridad
[Cómo manejas las credenciales: variables de entorno, Ansible Vault, etc. — NUNCA hardcodeadas]

## 📚 Resultados / Aprendizajes
[Ej: "Reduje el tiempo de backup de 20 dispositivos de 1 hora a 3 minutos"]
