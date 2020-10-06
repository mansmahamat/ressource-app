<template>
    <base-card>
        <base-button @click="setSelectedTab('stored-resources')">Ressources enrengistrées</base-button>
        <base-button @click="setSelectedTab('add-resources')">Ajouter une ressource</base-button>
    </base-card>
    <component :is="selectedTab"></component>
</template>

<script>
import StoredResources from './StoredResources';
import AddResources from './AddResource'

export default {
    components : {
        StoredResources,
        AddResources
    },
    data() {
        return {
            selectedTab : 'stored-resources'
        }
    },
    methods: {
        setSelectedTab(tab){
            this.selectedTab = tab;
        }
    },
}
</script>