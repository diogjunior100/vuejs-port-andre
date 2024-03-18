<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
              'Engenheiro Aeroespacial na UnB com especialização em Gestão de Projetos na FIA, trago uma sólida experiência internacional e nacional. Ao longo de 2 anos e 5 meses na Huawei Technologies, desempenhei papéis chave, incluindo Project Control Manager(Controlador de projetos) , liderando o planejamento financeiro e o ciclo completo de planejamento e implantação de projetos de telecomunicação.',
				},
				{
					id: 2,
					bio:
						'Anteriormente, na Brasal, destaquei-me como Analista de Risco, implementando a Gestão de Riscos e desenvolvendo políticas corporativas. Também atuei como Consultor de Projetos PMO na BR+ Comunicação, liderando melhorias nos processos de gestão e implementação de escritório de projetos (PMO).',
				},
        {
          id: 3,
          bio:
              'Minha carreira é marcada por desenvolvimento de habilidades em gestão de projetos tanto tradicional PMBOK (PMI) como em times ágeis (SCRUM) , liderança sob pressão, projetos interdisciplinares, apresentações executivas, relacionamento com diversos Stakeholders internos e externos . ',
        },
        {
          id: 4,
          bio:
              'Estou preparado para desafios inovadores no campo da gestão de projetos.',
        },
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/andre-foto-perfil"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
