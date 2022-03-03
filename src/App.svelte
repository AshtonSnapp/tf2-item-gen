<script lang="ts">
	import {
		Alert,
		Card,
		CardBody,
		CardHeader,
		Dropdown,
		DropdownItem,
		DropdownMenu,
		DropdownToggle,
		Nav,
		Navbar,
		NavbarBrand,
		Styles
	} from 'sveltestrap';

	// Item class.
	class Item {
		merc: "Scout" | "Soldier" | "Pyro" | "Demoman" | "Heavy" | "Engineer" | "Medic" | "Sniper" | "Spy";
		kind: string;
		attr: [string, boolean][];

		constructor(f: 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9) {
			switch (f) {
				case 1:
					this.merc = "Scout";
					break;
				case 2:
					this.merc = "Soldier";
					break;
				case 3:
					this.merc = "Pyro";
					break;
				case 4:
					this.merc = "Demoman";
					break;
				case 5:
					this.merc = "Heavy";
					break;
				case 6:
					this.merc = "Engineer";
					break;
				case 7:
					this.merc = "Medic";
					break;
				case 8:
					this.merc = "Sniper";
					break;
				case 9:
					this.merc = "Spy";
					break;
				default:
					break;
			}

			this.kind = "";
			this.attr = [];
		}
	}
	
	// An array of the items we have generated.
	let items: Item[] = [];

	// Scout
	function newScattergun() {
		const weapon = new Item(1);
		weapon.kind = "Scattergun";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newScoutPistol() {
		const weapon = new Item(1);
		weapon.kind = "Pistol";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newBat() {
		const weapon = new Item(1);
		weapon.kind = "Bat";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newScoutConsumable() {
		const weapon = new Item(1);
		weapon.kind = "Consumable";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newScoutThrowable() {
		const weapon = new Item(1);
		weapon.kind = "Throwable";

		// stuff goes here

		items.push(weapon);
		items = items;
	}

	// Soldier
	function newRocketLauncher() {
		const weapon = new Item(2);
		weapon.kind = "Rocket Launcher";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newSoldierShotgun() {
		const weapon = new Item(2);
		weapon.kind = "Shotgun";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newShovel() {
		const weapon = new Item(2);
		weapon.kind = "Shovel";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newSoldierBoots() {
		const weapon = new Item(2);
		weapon.kind = "Boots";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newBanner() {
		const weapon = new Item(2);
		weapon.kind = "Banner";

		// stuff goes here

		items.push(weapon);
		items = items;
	}

	// Pyro
	function newFlamethrower() {
		const weapon = new Item(3);
		weapon.kind = "Flamethrower";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newFlareGun() {
		const weapon = new Item(3);
		weapon.kind = "Flare Gun";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newAxe() {
		const weapon = new Item(3);
		weapon.kind = "Axe";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newPyroThrowable() {
		const weapon = new Item(3);
		weapon.kind = "Throwable";

		// stuff goes here

		items.push(weapon);
		items = items;
	}

	// Demoman
	function newGrenadeLauncher() {
		const weapon = new Item(4);
		weapon.kind = "Grenade Launcher";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newStickyLauncher() {
		const weapon = new Item(4);
		weapon.kind = "Stickybomb Launcher";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newBottle() {
		const weapon = new Item(4);
		weapon.kind = "Bottle";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newDemoBoots() {
		const weapon = new Item(4);
		weapon.kind = "Boots";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newShield() {
		const weapon = new Item(4);
		weapon.kind = "Shield";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newSword() {
		const weapon = new Item(4);
		weapon.kind = "Sword";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newDemoBack() {
		const weapon = new Item(4);
		weapon.kind = "Back Item";

		// stuff goes here

		items.push(weapon);
		items = items;
	}

	// Heavy
	function newMinigun() {
		const weapon = new Item(5);
		weapon.kind = "Minigun";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newHeavyShotgun() {
		const weapon = new Item(5);
		weapon.kind = "Shotgun";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newFists() {
		const weapon = new Item(5);
		weapon.kind = "Fists";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newHeavyConsumable() {
		const weapon = new Item(5);
		weapon.kind = "Consumable";

		// stuff goes here

		items.push(weapon);
		items = items;
	}

	// Engineer
	function newEngieShotgun() {
		const weapon = new Item(6);
		weapon.kind = "Shotgun";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newEngiePistol() {
		const weapon = new Item(6);
		weapon.kind = "Pistol";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newWrench() {
		const weapon = new Item(6);
		weapon.kind = "Wrench";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newPDA() {
		const weapon = new Item(6);
		weapon.kind = "PDA";

		// stuff goes here

		items.push(weapon);
		items = items;
	}

	// Medic
	function newSyringeGun() {
		const weapon = new Item(7);
		weapon.kind = "Syringe Gun";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newMediGun() {
		const weapon = new Item(7);
		weapon.kind = "Medi Gun";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newSaw() {
		const weapon = new Item(7);
		weapon.kind = "Saw";

		// stuff goes here

		items.push(weapon);
		items = items;
	}

	// Sniper
	function newSniperRifle() {
		const weapon = new Item(8);
		weapon.kind = "Sniper Rifle";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newSMG() {
		const weapon = new Item(8);
		weapon.kind = "SMG";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newMachete() {
		const weapon = new Item(8);
		weapon.kind = "Machete";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newBow() {
		const weapon = new Item(8);
		weapon.kind = "Bow";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newSniperThrowable() {
		const weapon = new Item(8);
		weapon.kind = "Throwable";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newSniperBack() {
		const weapon = new Item(8);
		weapon.kind = "Backpack";

		// stuff goes here

		items.push(weapon);
		items = items;
	}

	// Spy
	function newRevolver() {
		const weapon = new Item(9);
		weapon.kind = "Revolver";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newKnife() {
		const weapon = new Item(9);
		weapon.kind = "Knife";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newDisguiseKit() {
		const weapon = new Item(9);
		weapon.kind = "Disguise Kit";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newWatch() {
		const weapon = new Item(9);
		weapon.kind = "Watch";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
	function newSapper() {
		const weapon = new Item(9);
		weapon.kind = "Sabotage Item";

		// stuff goes here

		items.push(weapon);
		items = items;
	}
</script>

<Navbar color="dark" dark expand="md">
	<NavbarBrand>Ashton's TF2 Weapon Generator</NavbarBrand>
	<Nav class="ms-auto" navbar>
		<!-- Scout -->
		<Dropdown nav inNavbar>
			<DropdownToggle nav caret>Scout</DropdownToggle>
			<DropdownMenu end>
				<DropdownItem on:click={newScattergun}>Scattergun</DropdownItem>
				<DropdownItem on:click={newScoutPistol}>Pistol</DropdownItem>
				<DropdownItem on:click={newBat}>Bat</DropdownItem>
				<DropdownItem divider />
				<DropdownItem header>Alternatives</DropdownItem>
				<DropdownItem on:click={newScoutConsumable}>Consumable</DropdownItem>
				<DropdownItem on:click={newScoutThrowable}>Throwable</DropdownItem>
			</DropdownMenu>
		</Dropdown>

		<!-- Soldier -->
		<Dropdown nav inNavbar>
			<DropdownToggle nav caret>Soldier</DropdownToggle>
			<DropdownMenu end>
				<DropdownItem on:click={newRocketLauncher}>Rocket Launcher</DropdownItem>
				<DropdownItem on:click={newSoldierShotgun}>Shotgun</DropdownItem>
				<DropdownItem on:click={newShovel}>Shovel</DropdownItem>
				<DropdownItem divider />
				<DropdownItem header>Alternatives</DropdownItem>
				<DropdownItem on:click={newSoldierBoots}>Boots</DropdownItem>
				<DropdownItem on:click={newBanner}>Banner</DropdownItem>
			</DropdownMenu>
		</Dropdown>

		<!-- Pyro -->
		<Dropdown nav inNavbar>
			<DropdownToggle nav caret>Pyro</DropdownToggle>
			<DropdownMenu end>
				<DropdownItem on:click={newFlamethrower}>Flamethrower</DropdownItem>
				<DropdownItem on:click={newFlareGun}>Flare Gun</DropdownItem>
				<DropdownItem on:click={newAxe}>Axe</DropdownItem>
				<DropdownItem divider />
				<DropdownItem header>Alternatives</DropdownItem>
				<DropdownItem on:click={newPyroThrowable}>Throwable</DropdownItem>
			</DropdownMenu>
		</Dropdown>

		<!-- Demoman -->
		<Dropdown nav inNavbar>
			<DropdownToggle nav caret>Demoman</DropdownToggle>
			<DropdownMenu end>
				<DropdownItem on:click={newGrenadeLauncher}>Grenade Launcher</DropdownItem>
				<DropdownItem on:click={newStickyLauncher}>Sticky Launcher</DropdownItem>
				<DropdownItem on:click={newBottle}>Bottle</DropdownItem>
				<DropdownItem divider />
				<DropdownItem header>Demoknight</DropdownItem>
				<DropdownItem on:click={newDemoBoots}>Boots</DropdownItem>
				<DropdownItem on:click={newShield}>Shield</DropdownItem>
				<DropdownItem on:click={newSword}>Sword</DropdownItem>
				<DropdownItem divider />
				<DropdownItem header>Alternatives</DropdownItem>
				<DropdownItem on:click={newDemoBack}>Back</DropdownItem>
			</DropdownMenu>
		</Dropdown>

		<!-- Heavy -->
		<Dropdown nav inNavbar>
			<DropdownToggle nav caret>Heavy</DropdownToggle>
			<DropdownMenu end>
				<DropdownItem on:click={newMinigun}>Minigun</DropdownItem>
				<DropdownItem on:click={newHeavyShotgun}>Shotgun</DropdownItem>
				<DropdownItem on:click={newFists}>Fists</DropdownItem>
				<DropdownItem divider />
				<DropdownItem header>Alternatives</DropdownItem>
				<DropdownItem on:click={newHeavyConsumable}>Consumable</DropdownItem>
			</DropdownMenu>
		</Dropdown>

		<!-- Engineer -->
		<Dropdown nav inNavbar>
			<DropdownToggle nav caret>Engineer</DropdownToggle>
			<DropdownMenu end>
				<DropdownItem on:click={newEngieShotgun}>Shotgun</DropdownItem>
				<DropdownItem on:click={newEngiePistol}>Pistol</DropdownItem>
				<DropdownItem on:click={newWrench}>Wrench</DropdownItem>
				<DropdownItem on:click={newPDA}>PDA</DropdownItem>
			</DropdownMenu>
		</Dropdown>

		<!-- Medic -->
		<Dropdown nav inNavbar>
			<DropdownToggle nav caret>Medic</DropdownToggle>
			<DropdownMenu end>
				<DropdownItem on:click={newSyringeGun}>Syringe Gun</DropdownItem>
				<DropdownItem on:click={newMediGun}>Medi Gun</DropdownItem>
				<DropdownItem on:click={newSaw}>Saw</DropdownItem>
			</DropdownMenu>
		</Dropdown>

		<!-- Sniper -->
		<Dropdown nav inNavbar>
			<DropdownToggle nav caret>Sniper</DropdownToggle>
			<DropdownMenu end>
				<DropdownItem on:click={newSniperRifle}>Sniper Rifle</DropdownItem>
				<DropdownItem on:click={newSMG}>SMG</DropdownItem>
				<DropdownItem on:click={newMachete}>Machete</DropdownItem>
				<DropdownItem divider />
				<DropdownItem header>Alternatives</DropdownItem>
				<DropdownItem on:click={newBow}>Bow</DropdownItem>
				<DropdownItem on:click={newSniperThrowable}>Throwable</DropdownItem>
				<DropdownItem on:click={newSniperBack}>Backpack</DropdownItem>
			</DropdownMenu>
		</Dropdown>

		<!-- Spy -->
		<Dropdown nav inNavbar>
			<DropdownToggle nav caret>Spy</DropdownToggle>
			<DropdownMenu end>
				<DropdownItem on:click={newRevolver}>Revolver</DropdownItem>
				<DropdownItem on:click={newKnife}>Knife</DropdownItem>
				<DropdownItem on:click={newDisguiseKit}>Disguise Kit</DropdownItem>
				<DropdownItem on:click={newWatch}>Watch</DropdownItem>
				<DropdownItem on:click={newSapper}>Sabotage Item</DropdownItem>
			</DropdownMenu>
		</Dropdown>
	</Nav>
</Navbar>

<p><br>Hello! I tried my hand at making a TF2 weapon generator. It tries to make balanced weapons, but nothing is perfect and that goes for this too.</p>

{#each items as item}
	<Card>
		<CardHeader>New {item.kind} for the {item.merc}</CardHeader>
		<CardBody>
			{#each item.attr as a}
				{#if a[1]}
					<Alert color="primary">{a[0]}</Alert>
				{:else}
					<Alert color="danger">{a[0]}</Alert>
				{/if}
			{/each}
		</CardBody>
	</Card>
{:else}
	<Alert color="info">
		<h4>No weapons!</h4>
		<p>Click on a weapon type under each class to create weapons. This alert will go away once you have some weapons generated.</p>
	</Alert>
{/each}

<Styles />