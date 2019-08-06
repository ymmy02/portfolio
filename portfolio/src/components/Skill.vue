<template>
    <div id="skill">
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
                    content: 'C/C++, Java, Python, C#, Fortran, Go, HTML, JavaScript, TypeScript, R, Bashscript',
                    images: [
                        require('@/assets/programming-language/java.png'),
                        require('@/assets/programming-language/python.png'),
                        require('@/assets/programming-language/javascript.png'),
                        require('@/assets/programming-language/golang.png'),
                    ]
                },
                {
                    title: 'Database',
                    content: 'MySQL, PostgreSQL, MongoDB',
                    images: [
                        require('@/assets/database/mysql.png'),
                        require('@/assets/database/postgresql.png'),
                        require('@/assets/database/mongodb.png'),
                    ]
                },
                {
                    title: 'Backend',
                    content: 'Django, Node',
                    images: [
                        require('@/assets/backend/django.png'),
                        require('@/assets/backend/nodejs.png'),
                    ]
                },
                {
                    title: 'Frontend',
                    content: 'Vue.js, React.js, jQuery',
                    images: [
                        require('@/assets/frontend/vuejs.png'),
                        require('@/assets/frontend/reactjs.png'),
                        require('@/assets/frontend/jquery.png'),
                    ]
                },
                {
                    title: 'Machine Learning',
                    content: 'Keras, TensorFlow, scikit-learn',
                    images: [
                        require('@/assets/machine-learning/keras.png'),
                        require('@/assets/machine-learning/tensorflow.png'),
                        require('@/assets/machine-learning/sklearn.png'),
                    ]
                },
                {
                    title: 'Others',
                    content: 'GCP, Docker, Parallelization, Optimization, English, etc...',
                    images: [
                        require('@/assets/others/gcp.png'),
                        require('@/assets/others/firebase.png'),
                        require('@/assets/others/docker.png'),
                    ]
                },
            ]
        }
    }
}
</script>
