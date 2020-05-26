<template>
    <b-navbar>
        <template slot="brand">
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img
                    src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"
                    alt="Lightweight UI components for Vue.js based on Bulma"
                >
            </b-navbar-item>
        </template>
        <template slot="start">
            <b-navbar-item href="#">
                Home
            </b-navbar-item>
            <b-navbar-item href="#">
                Documentation
            </b-navbar-item>
            <b-navbar-dropdown label="Info">
                <nuxt-link to="/users">
                <b-navbar-item href="#">
                    Usuários
                </b-navbar-item>
                </nuxt-link>
                <b-navbar-item href="#">
                    Contato
                </b-navbar-item>
            </b-navbar-dropdown>
        </template>

       
    </b-navbar>
</template>