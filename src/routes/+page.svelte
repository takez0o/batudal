<script lang="ts">
	import { assets } from '$app/paths';

	let reach_link = 'https://twitter.com/takez0_o';

	let skills = [
		{
			name: 'Ideation',
			description: 'Ideation; business modeling, strategy',
			icon: 'icons/idea.svg'
		},
		{
			name: 'Design',
			description: 'Design; branding,ui,ux',
			icon: 'icons/design.svg'
		},
		{
			name: 'Development',
			description: 'Fullstack development',
			icon: 'icons/development.svg'
		},
		{
			name: 'Soft Skills',
			description: 'Hiring, training, management',
			icon: 'icons/softskills.svg'
		}
	];
	let attempts = [
		{
			title: 'e-liner',
			success: false,
			description:
				'E-Liner builds upon the idea of a digital warehouse that solves the inefficiency problems in LTL transports. E-Liner is a software company modeled around a typical platform business; matching solo truck businesses with customers in need of cheap and fast cross-country transportation.',
			tags: [
				{
					title: 'DEAD 💀',
					style: 'color: var(--color-primary);'
				}
			],
			achievements: [
				'Branding assets',
				'Routing algorithm POC',
				'Company formation',
				'Concierge bootstrap'
			],
			post_mortem:
				'Stakeholders had completely different visions for the product. It went unto being a hardware project for 5+ years, seeking a solution via hybrid-fuel technology for the transition period of truck transportation.'
		},
		{
			title: 'innhof',
			link: 'https://decoded-files.fra1.cdn.digitaloceanspaces.com/takezo%2Finnhof.pdf',
			link_tag: 'brochure/innhof',
			success: false,
			description:
				"We envision becoming the leading worldwide community of innovators, where individuals and businesses of all sizes cocreate a better future. Our joint efforts are focused on equipping InnHof's global members with enabling tailor- made programs & services, modern technologies in development and the most inspiring spaces to work at, thus allowing the collaborative creation of brand-new values at an increasing pace.",
			tags: [
				{
					title: 'DEAD 💀',
					style: 'color: var(--color-primary);'
				}
			],
			achievements: [
				'Acquisition of physical space',
				'Office modules POC',
				'Branding, company formation',
				'Opening party',
				'Local community'
			],
			post_mortem:
				'Innhof was built on an opporunity instead of a solid market scan. It had disadvantages from the start that we could perhaps overcome. We realised that the local population will not be able to sustain the space we were handed initially.'
		},
		{
			title: 'guuru',
			success: false,
			description:
				"Guuru was an initiative to educate and on-board traditional companies to blockchain. We travelled to various events and collected connections all over the country. Although it didn't go far, it's where my blockchain journey started.",
			tags: [
				{
					title: 'DEAD 💀',
					style: 'color: var(--color-primary);'
				}
			],
			achievements: [
				'Attended local crypto events',
				'Networking with local blockchain companies',
				'Branding, exhibition booth'
			],
			post_mortem:
				'We were able to onboard a few companies to the blockchain space, however, we were not able to scale the business.'
		},
		{
			title: 'neustrukt',
			link: 'https://github.com/takez0o/neustrukt',
			link_tag: 'github/neustrukt',
			success: false,
			description:
				'Neustrukt aimed to bring a radical change in house production. Starting from software up to the final product via flexible fabricated modules; Neustrukt allowed for a more efficient and sustainable lifecycle for construction industry.',
			tags: [
				{
					title: 'DEAD 💀',
					style: 'color: var(--color-primary);'
				}
			],
			achievements: [
				'ACM technology',
				'ACM trademarking',
				'Office space',
				'Company formation',
				'First customers'
			],
			post_mortem:
				'Neustrukt is a much needed solution for todays construction industry. However, it needs a lengthy runway to achieve process excellency. We decided to scale down and focus to the core design system and intermediate products.'
		},
		{
			title: 'siradaki',
			success: false,
			description:
				'Siradaki is a consumer electronics rental platform that aimed to provide a more sustainable flexible and affordable way obtain to consumer electronics. We aimed to provide subscripton models that allowed people to experience electronics without the need to purchase them.',
			tags: [
				{
					title: 'DEAD 💀',
					style: 'color: var(--color-primary);'
				}
			],
			achievements: [
				'Team formation',
				'Business model design',
				'Feasibility study',
				'Branding assets',
				'UI/Frontend components',
				'Investor attraction',
				'Strategic partnerships'
			],
			post_mortem:
				'Team did not want to work on the operational hurdle of the business and decided to pursue different opportunities on Web3 independent of physical operations like supply chain.'
		},
		{
			title: 'spintop network',
			success: true,
			link: 'https://www.spintop.network',
			link_tag: 'spintop.network',
			description:
				'Spintop is the next generation blockchain gaming hub that aims to utilize the new tools of web3 to offer a comprehensive experience for players, traders and investors. In Spintop, we aspire to guide, discuss and supply through blockchain gaming. The ecosystem is designed as a gaming hub that allows players to exchange their tokens, NFTs, and reviews.',
			tags: [
				{
					title: 'RUNNING 👣',
					style: 'color: var(--color-walking);'
				}
			],
			achievements: ['120k monthly traffic', '$200m volume on contracts', '20m valuation']
		},
		{
			title: 'txt',
			success: false,
			description:
				'TXT Project is a series of experiments that aims to explore the possibilities of blockchain technology in the art world. It involves automated twitter bots, 128+ stories, and multi-level mechanics running on the Ethereum blockchain.',
			tags: [
				{
					title: 'DEAD 💀',
					style: 'color: var(--color-primary);'
				}
			],
			achievements: [
				'GreedyDAO: a user owned on-chain casino',
				'x0x: decision-based minting experience',
				'w4ll: a twitter bot that streams user-inputs on-chain'
			],
			post_mortem:
				"None of them were advertised. It started as a project to learn EVM in and out, didn't spend much energy to market it"
		},
		{
			title: 'deadly games',
			link: 'https://github.com/deadly-games',
			link_tag: 'github/deadly-games',
			success: false,
			description:
				'Deadly Games is a series of 7 games, each inspired by one of the Deadly Sins. Main idea was to create a gamified, story-backed minting experience. It involved cutting-edge web3 technologies to create a unique experience for the players on StarkNET.',
			tags: [
				{
					title: 'DEAD 💀',
					style: 'color: var(--color-primary);'
				}
			],
			achievements: [
				'Team formation',
				'Landing page',
				'Solidity contracts',
				'Cairo contracts',
				'Demo game',
				'Community growth',
				'Investor atraction'
			],
			post_mortem:
				'Break-up between founders due to emotional responses. Later on, project got discontinued as main team moved on to other projects.'
		},
		{
			title: 'fungible future',
			success: false,
			link: 'https://www.fungiblefuture.com',
			link_tag: 'fungiblefuture.com',
			description:
				'Fungible future offers a new way of liquidifying your most illiquid assets. Underyling protocol provides a trustless framework to share future profits and distributes earnings to token holders.',
			tags: [
				{
					title: 'DEAD 💀',
					style: 'color: var(--color-primary);'
				}
			],
			achievements: ['Demo application', 'Branding assets', 'Solidity contracts'],
			post_mortem:
				"We had problems listing on Opensea with contracts. Without Opensea traffic, project doesn't offer much value to the users."
		},
		{
			title: 'nether finance',
			success: false,
			link: 'https://www.nether.finance',
			link_tag: 'nether.finance',
			description:
				'Nether Finance is a decentralized protocol that allows users to stake, lock and vest their native tokens. It is focused on post-merge staking ecosystem, providing a decentralized alternative against the current monopolistic staking providers. ',
			tags: [
				{
					title: 'DEAD 💀',
					style: 'color: var(--color-primary);'
				}
			],
			achievements: [
				'UI/Frontend components',
				'Solidity contracts',
				'Branding assets',
				'Social media presence'
			],
			post_mortem:
				"Projects with similar models were struggling. We tried to patch the wrongs of the model but finally decided that it's too experimental for the zeitgeist."
		},
		{
			title: 'decoded labs',
			success: true,
			link: 'https://www.decoded-labs.com',
			link_tag: 'decoded-labs.com',
			description:
				'Decoded Labs is a developer collective committed to safeguard your ventures into the ambigous decentralized world.',
			tags: [
				{
					title: 'IN PROGRESS 🐝',
					style: 'color: var(--color-incubating);'
				}
			],
			achievements: ['Branding assets', 'Landing page', 'Developer blog', 'First customers']
		},
		{
			title: 'microcolonies',
			success: true,
			link: 'https://www.microcolonies.com',
			link_tag: 'microcolonies.com',
			description:
				'"Microcolonies" allows you to simultaneously experience game, art, nature, and finance in the decentralized world. This unique experience will give you the pleasure of a game where nature is the architect, art is the prize, and money is the result.',
			tags: [
				{
					title: 'IN PROGRESS 🐝',
					style: 'color: var(--color-incubating);'
				}
			],
			achievements: ['Demo application', 'Physical sculpture', 'Branding assets', 'Team formation']
		},
		{
			title: 'honestwork',
			success: true,
			link: 'https://www.honestwork.app',
			link_tag: 'honestwork.app',
			description:
				'HonestWork connects clients with top-rated blockchain experts, including copywriters, developers, and designers.',
			tags: [
				{
					title: 'IN PROGRESS 🐝',
					style: 'color: var(--color-incubating);'
				}
			],
			achievements: [
				'Demo application',
				'Customer interviews',
				'Branding assets',
				'Team formation',
				'Solidity contracts'
			]
		}
	];
	$: attempts_reversed = attempts.slice().reverse();
</script>

<svelte:head>
	<title>Batu Dal</title>
	<meta name="description" content="Batu Dal's personal website about startup attempts" />
	<meta name="viewport" content="width=device-width, initial-scale=1" />
	<link rel="icon" type="image/png" href={`${assets}/favicon.png`} />
</svelte:head>

<main>
	<div class="background-wrapper">
		<div class="background-container">
			<img src={`${assets}/takezo.webp`} alt="takezo" />
		</div>
	</div>
	<div class="hero-container">
		<div class="content-container">
			<h1><span>Hi, </span>I'm Batu.</h1>
			<div style="height:24px" />
			<p>I'm an entrepreneur.</p>
			<div style="height:24px" />
			<p>I usually do all of these in a project;</p>
			<div style="height:12px" />
			{#each skills as skill}
				<div class="skills-container">
					<div class="skill">
						<img src={`${assets}/${skill.icon}`} alt={skill.name} />
						<div style="width:12px" />
						<p>{skill.description}</p>
					</div>
				</div>
			{/each}
			<div style="height:24px" />
			<p>And <span><strong>I fail a lot.</strong></span></p>
			<div style="height:24px" />
			<div class="status">
				<div class="tag">
					<h4><span>{attempts.length} </span>ATTEMPTS</h4>
				</div>
				<div style="width:20px" />
				<img src={`${assets}/icons/arrow.svg`} alt="arrow" />
				<div style="width:20px" />
				<div class="tag">
					<h4><span>{attempts.filter((a) => a.success == false).length} </span>FAILURES</h4>
				</div>
			</div>
			<div style="height:24px" />
			<p>Scroll to see my hall of shame.</p>
			<p>
				Feel free to <span
					><a href={reach_link} target="_blank" rel="noreferrer">reach out to me.</a></span
				>
			</p>
		</div>
	</div>
	<div class="attempts-container">
		{#each attempts_reversed as attempt, i}
			<div class="card">
				<div class="card-header">
					<h2>{attempt.title}</h2>
					<div class="tags">
						{#each attempt.tags as tag, j}
							<div class="tag">
								<h4 style={tag.style}>{tag.title}</h4>
							</div>
							{#if j !== attempt.tags.length - 1}
								<div style="width:8px" />
							{/if}
						{/each}
					</div>
				</div>
				{#if attempt.link}
					<div style="height:12px" />
					<div class="tag-link">
						<a href={attempt.link} target="_blank" rel="noreferrer"><h4>{attempt.link_tag}</h4></a>
					</div>
				{/if}
				<div class="divider-large" />
				<h3>ABSTRACT</h3>
				<div class="divider-small" />
				<p>{attempt.description}</p>
				<div class="divider-large" />
				<h3>PROGRESS</h3>
				<div class="divider-small" />
				{#each attempt.achievements as achievement}
					<div class="skills-container">
						<div class="skill">
							<img src={`${assets}/icons/check.svg`} alt="Achievements" />
							<div style="width:12px" />
							<p>{achievement}</p>
						</div>
					</div>
				{/each}
				{#if attempt.post_mortem}
					<div class="divider-large" />
					<h3>POST-MORTEM</h3>
					<div class="divider-small" />
					<p>{attempt.post_mortem}</p>
					{#if i !== attempts.length - 1}
						<div class="divider-small" />
					{/if}
				{/if}
			</div>
			{#if i !== attempts.length - 1}
				<div class="divider-large" />
			{/if}
		{/each}
	</div>
	<div class="divider-large" />
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.background-wrapper {
		position: fixed;
		top: 0;
		left: 0;
		width: 100vw;
		height: 100vh;
		z-index: -1;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.background-container {
		max-width: 920px;
		display: flex;
		flex-direction: row;
		justify-content: flex-end;
		/* overflow-x: hidden; */
	}
	.background-container img {
		width: 100%;
		height: calc(100vh - 64px);
		object-fit: scale-down;
		margin-right: -240px;
	}
	.hero-container {
		height: calc(100vh - 64px);
		width: 100vw;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.content-container {
		max-width: 920px;
		width: 100%;
		display: flex;
		flex-direction: column;
		justify-content: flex-start;
		margin-top: 64px;
	}
	.skills-container {
		display: flex;
		flex-direction: column;
		justify-content: flex-start;
		align-items: flex-start;
		margin-left: 12px;
		width: 100%;
	}
	.skill {
		display: flex;
		flex-direction: row;
		justify-content: flex-start;
		align-items: center;
	}
	.status {
		display: flex;
		flex-direction: row;
		justify-content: flex-start;
		align-items: center;
	}
	.attempts-container {
		width: 100%;
		display: flex;
		flex-direction: column;
		justify-content: flex-start;
		align-items: center;
	}
	.card-header {
		width: 100%;
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
	}
	.tags {
		display: flex;
		flex-direction: row;
		justify-content: flex-start;
		align-items: center;
	}
	.divider-large {
		height: 48px;
	}
	.divider-small {
		height: 16px;
	}
	@media only screen and (max-width: 960px) {
		.card-header {
			flex-wrap: wrap;
			align-items: flex-start;
			gap: 8px;
		}
		.status > img {
			width: 57px;
		}
		.background-container {
			margin-right: 160px;
			width: max-content;
		}
		.hero-container {
			width: 95%;
		}
		.divider-large {
			height: 32px;
		}
		.divider-small {
			height: 12px;
		}
	}
</style>
