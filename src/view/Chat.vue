<template>
    <el-row class="chat-main">

        <el-row class="header" justify="space-between" align="middle">
            <span>房间号：</span>
            <span>文件传输助手(在线1人)</span>
            <span>昵称：</span>
        </el-row>

        <el-row class="body">
            <el-tag class="ml-2" type="info">你好啊</el-tag>
            <el-tag>也太厉害了</el-tag>
        </el-row>

        <el-row class="footer">
            <el-col>
                <el-space :size="8">
                    <el-tag class="ml-2" type="success">生成二维码</el-tag>
                    <el-tag class="ml-2" type="success">加入房间</el-tag>
                    <el-tag class="ml-2" type="success">分享房间</el-tag>
                </el-space>
            </el-col>
            <el-col class="input">
                <el-input placeholder="Please input">
                    <template #suffix>
                        <el-button circle>
                            <template #icon>
                                <el-icon size="32">
                                    <CirclePlusFilled />
                                </el-icon>
                            </template>
                        </el-button>
                        <el-button type="primary">发送</el-button>
                    </template>
                </el-input>
            </el-col>

        </el-row>

    </el-row>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import { CirclePlusFilled } from '@element-plus/icons-vue'


</script>

<style scoped lang="less">
.chat-main {
    height: 100vh;
    min-height: 100vh;
    padding: 0.5rem;
    flex-direction: column;
    border: 1px solid #ccc;
    border-radius: 0.25rem;

    .header {
        height: 3rem;
        font-size: 0.75rem;
        padding: 0.5rem;
        color: #fafafa;
        background-color: #409eff;
        border-radius: 0.25rem;
    }

    .body {
        flex: 1 1 auto;

        margin: 0.25rem;
    }

    .footer {
        width: 100%;
        height: 4rem;

        :deep(.el-input__wrapper) {
            padding: 0.1rem 0 0.1rem 1rem;
        }
    }
}
</style>
