<template>
	<a-layout>
		<Header />
		<a-layout>
			<Aside />
			<a-layout-content>
				<div
					:style="{
						background: '#c6d7eb',
						padding: '24px',
						minHeight: 'calc(100vh - 64px)'
					}"
				>
					<router-view></router-view>
				</div>
			</a-layout-content>
		</a-layout>

		<a-layout-footer style="text-align: center">
			Ссслыка
		</a-layout-footer>
	</a-layout>
</template>

<script setup>
import Header from './components/Header.vue'
import Aside from './components/Aside.vue'
</script>
