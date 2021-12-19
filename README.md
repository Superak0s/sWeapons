# sVehicles
 
## Installation
- Download the resource and copy the files to **resources/sWeapons**.
- Open your server.cfg and add `ensure sWeapons` to the resource list.
- (Re)start your server.

## Usage
- The pack includes: ak47, g36c, hk416a5, lr300, m4damage edition, m4white, m16a1, phantom, stg44
- To spawn the weapons you need to go in to vMenu, player options, weapon options, spawn weapons and for the weapon name:

| Name                | Spawn Code                |
|---------------------|---------------------------|
| ak47                | WEAPON_AK47               |
| g36c                | WEAPON_G36C               |
| hk416a5             | WEAPON_HK416A5            |
| lr300               | WEAPON_LR300              |
| m4 damage edition   | WEAPON_M4DAMAGE-EDITION   |
| m4 white            | WEAPON_M4WHITE            |
| m16a1               | WEAPON_M16A1              |
| phantom             | WEAPON_PHANTOM            |
| stg44               | WEAPON_STG44              |

## Give weapon command
- In order to spawn the weapon with the /giveweapon command you need to go to es_extended/config.weapons.lua and under the advanced rifle place this

```lua
{
		name = 'WEAPON_STG44',
		label = _U('weapon_stg44'),
		ammo = {label = _U('ammo_rounds'), hash = `AMMO_RIFLE`},
		tints = Config.DefaultWeaponTints,
		components = {
			{name = 'clip_default', label = _U('component_clip_default'), hash = `COMPONENT_STG44_CLIP_01`}
		}
	},
	{
		name = 'WEAPON_AK47',
		label = _U('weapon_ak47'),
		ammo = {label = _U('ammo_rounds'), hash = `AMMO_RIFLE`},
		tints = Config.DefaultWeaponTints,
		components = {
			{name = 'clip_default', label = _U('component_clip_default'), hash = `COMPONENT_AK47_CLIP_01`}
		}
	},
	{
		name = 'WEAPON_G36C',
		label = _U('weapon_g36c'),
		ammo = {label = _U('ammo_rounds'), hash = `AMMO_RIFLE`},
		tints = Config.DefaultWeaponTints,
		components = {
			{name = 'clip_default', label = _U('component_clip_default'), hash = `COMPONENT_G36C_CLIP_01`}
		}
	},
	{
		name = 'WEAPON_HK416A5',
		label = _U('weapon_hk416a5'),
		ammo = {label = _U('ammo_rounds'), hash = `AMMO_RIFLE`},
		tints = Config.DefaultWeaponTints,
		components = {
			{name = 'clip_default', label = _U('component_clip_default'), hash = `COMPONENT_HK416A5_CLIP_01`}
		}
	},
	{
		name = 'WEAPON_LR300',
		label = _U('weapon_lr300'),
		ammo = {label = _U('ammo_rounds'), hash = `AMMO_RIFLE`},
		tints = Config.DefaultWeaponTints,
		components = {
			{name = 'clip_default', label = _U('component_clip_default'), hash = `COMPONENT_LR300_CLIP_01`}
		}
	},
	{
		name = 'WEAPON_M4DAMAGE-EDITION',
		label = _U('weapon_m4damage'),
		ammo = {label = _U('ammo_rounds'), hash = `AMMO_RIFLE`},
		tints = Config.DefaultWeaponTints,
		components = {
			{name = 'clip_default', label = _U('component_clip_default'), hash = `COMPONENT_M4DAMAGE-EDITION_CLIP_01`}
		}
	},
	{
		name = 'WEAPON_M4WHITE',
		label = _U('weapon_m4white'),
		ammo = {label = _U('ammo_rounds'), hash = `AMMO_RIFLE`},
		tints = Config.DefaultWeaponTints,
		components = {
			{name = 'clip_default', label = _U('component_clip_default'), hash = `COMPONENT_M4WHITE_CLIP_01`}
		}
	},
	{
		name = 'WEAPON_M16A1',
		label = _U('weapon_m16a1'),
		ammo = {label = _U('ammo_rounds'), hash = `AMMO_RIFLE`},
		tints = Config.DefaultWeaponTints,
		components = {
			{name = 'clip_default', label = _U('component_clip_default'), hash = `COMPONENT_M16A1_CLIP_01`}
		}
	},
	{
		name = 'WEAPON_PHANTOM',
		label = _U('weapon_phantom'),
		ammo = {label = _U('ammo_rounds'), hash = `AMMO_RIFLE`},
		tints = Config.DefaultWeaponTints,
		components = {
			{name = 'clip_default', label = _U('component_clip_default'), hash = `COMPONENT_PHANTOM_CLIP_01`}
		}
	},
```

- After you do that, go to es_extended/locales/ the language you are using and place under advanced rifle this:

```lua
  ['weapon_ak47'] = 'AK47',
  ['weapon_g36c'] = 'G36C',
  ['weapon_hk416a5'] = 'HK416A5',
  ['weapon_lr300'] = 'LR300',
  ['weapon_m4damage'] = 'M4DAMAGE',
  ['weapon_m4white'] = 'M4WHITE',
  ['weapon_m16a1'] = 'M16A1',
  ['weapon_phantom'] = 'PHANTOM',
  ['weapon_stg44'] = 'STG44',
  ```

 - Now you can spawn the weapons with the command /giveweapon