
<script>
 /* eslint-disable */
import AboutSkillSingle from './AboutSkillSingle.vue';
 /* eslint-disable */
export default {
	 /* eslint-disable */
	components: {
		AboutSkillSingle,
	},
	data: () => {
		return {
			SkillsHeading: 'Some of my work experince ',
			skills: [
				{
					id: 1,
					title: 'HTMl',
					img: require('@/assets/images/brands/html.png'),
				},
				{
					id: 2,
					title: 'graphic',
					 img: require('@/assets/images/brands/graphic.jpeg'),
				},
				{
					id: 3,
					title: 'Bootstrap',
					img: require('@/assets/images/brands/bootstrap.png'),
				},
				{
					id: 4,
					title: 'pinia',
					img: require('@/assets/images/brands/pinia.png'),
				},
				{
					id: 5,
					title: 'vuejs',
					img: require('@/assets/images/brands/vuejs.png'),
				},
				{
					id: 6,
					title: 'taillwind',
					img: require('@/assets/images/brands/tailwind.jpg'),
				},
				
				{
					id: 7,
					title: 'css',
					img: require('@/assets/images/brands/css.jpg'),
				},
			],
		};
	},
};
</script>

<template>
	<div class="mt-10 sm:mt-20">
		<p
			class="font-general-medium text-2xl sm:text-3xl text-primary-dark dark:text-primary-light"
		>
			{{ SkillsHeading }}
		</p>
		<div class="grid grid-cols-2 sm:grid-cols-4 mt-10 sm:mt-14 gap-2">
			<AboutSkillSingle
				v-for="skill in skills"
				:key="skill.id"
				:skill="skill"
			/>
		</div>
	</div>
</template>
