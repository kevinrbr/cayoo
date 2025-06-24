<script setup lang="ts">
import { Copy } from 'lucide-vue-next'
import { Button } from '@/components/ui/button';
import {
  Dialog,
  DialogClose,
  DialogContent,
  DialogDescription,
  DialogFooter,
  DialogHeader,
  DialogTitle,
  DialogTrigger,
} from '@/components/ui/dialog'
import { Input } from '@/components/ui/input'
import { Label } from '@/components/ui/label'
</script>

<template>
  <Dialog>
    <DialogTrigger as-child>
      <Button variant="outline">
        Share
      </Button>
    </DialogTrigger>
    <DialogContent class="sm:max-w-md">
      <DialogHeader class="mb-4">
        <DialogTitle class="text-primary font-satoshi font-bold text-5xl">cayoo</DialogTitle>
        <DialogDescription>
          Je me connecte pour gérer mes réservations.
        </DialogDescription>
      </DialogHeader>
      <div class="flex items-center space-x-2">
        <div class="grid flex-1 gap-2">
          <Label>
            Email
          </Label>
          <Input
            id="link"
            default-value="https://shadcn-vue.com/docs/installation"
            read-only
          />
        </div>
      </div>
      <div class="flex items-center space-x-2 mt-4">
        <div class="grid flex-1 gap-2">
          <Label>
            Mot de passe
          </Label>
          <Input
            id="link"
            default-value="https://shadcn-vue.com/docs/installation"
            read-only
          />
        </div>
      </div>
      <Label class="underline justify-end">
        Mot de passe oublié
      </Label>
      <DialogFooter class="!flex-col items-start space-y-2 items-center">
        <DialogClose as-child class="mt-6">
          <Button type="button" size="full">
            Continuer
          </Button>
        </DialogClose>
        <a class="underline cursor-pointer text-sm">
          Créer un compte
        </a>
      </DialogFooter>
    </DialogContent>
  </Dialog>
</template>