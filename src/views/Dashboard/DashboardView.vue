<script setup lang="ts">
import DashboardSidebar from "@/components/Dashboard/Layout/DashboardSidebar.vue";
import DashboardTopbar from "@/components/Dashboard/Layout/DashboardTopbar.vue";
import DashboardStatisticCard from "@/components/Dashboard/DashboardStatisticCard.vue";
import DashboardGrowthCard from "@/components/Dashboard/DashboardGrowthCard.vue";
import DashboardTransactionCard from "@/components/Dashboard/DashboardTransactionCard.vue";
import DashboardGoalCard from "@/components/Dashboard/DashboardGoalCard.vue";
import DashboardChallengeCard from "@/components/Dashboard/DashboardChallengeCard.vue";
</script>
<template>
    <div class="flex min-h-screen pb-10">
        <DashboardSidebar />
        <main class="lg:pt-[50px] lg:px-[50px] p-4 w-full lg:border-l lg:border-l-borderLight">
            <DashboardTopbar/>
            <div class="flex flex-col lg:flex-row gap-[30px]">
                <section class="w-full flex flex-col gap-[30px]">
                <!-- Statistic card -->
                <DashboardStatisticCard/>
                <!-- Your growth -->
                <DashboardGrowthCard/>
                <!-- Latest Transaction -->
                <DashboardTransactionCard/>
                </section>
                <section class="lg:max-w-[300px] w-full h-max mb-[30px] bg-subtleGrey rounded-2xl p-4">
                <!-- Goal Card -->
                <DashboardGoalCard/>
                <!-- Challenge Card -->
                <DashboardChallengeCard/>
                </section>
            </div>
        </main>
    </div>
</template>