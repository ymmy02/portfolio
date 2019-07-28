<template>
    <div class="skill">
        <h2 class="content-title font-weight-regular mt-4 ml-4">
            <v-icon>mdi-laptop</v-icon>
            Skill
        </h2>
        <v-layout wrap>
            <SkillCard 
                v-for="card in cards"
                :key="card.title"
                :title="card.title"
                :content="card.content"
                :images="card.images"
            />
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
                {
                    title: 'Programming Language',
                    content: 'C/C++, Python, Javascript, Java',
                    images: [
                        require('../assets/programming-language/python.png'),
                        require('../assets/programming-language/javascript.png'),
                        require('../assets/programming-language/golang.png'),
                    ]
                },
                {
                    title: 'Backend',
                    content: 'Django, Node'
                },
                {
                    title: 'Frontend',
                    content: 'Vue.js, React.js, jQuery'
                }
            ]
        }
    }
}
</script>
