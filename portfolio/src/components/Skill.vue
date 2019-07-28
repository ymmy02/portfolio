<template>
    <div class="skill">
        <h2 class="content-title font-weight-regular mt-4 ml-4">
            <v-icon>mdi-laptop</v-icon>
            Skill
        </h2>
        <v-layout wrap>
            <SkillCard v-for="card in cards" :key="card.title" />
        </v-layout>
    </div>
</template>

<script>
import SkillCard from './SkillCard';

export default {
    name: 'Skill',
    components: {
        SkillCard
    },
    data: () => {
        return {
            cards: [
                {title: 'Programming Language'},
                {title: 'Backend'},
                {title: 'Frontend'}
            ]
        }
    }
}
</script>
