# Tailwind CSS @apply Directive Error with Vue.js/React

This repository demonstrates a common error encountered when using Tailwind CSS's `@apply` directive within Vue.js or React applications. The issue stems from a conflict between Tailwind's compilation process and the framework's CSS handling.

## Problem

The `@apply` directive, while convenient, can lead to errors if not used correctly within a framework context. This usually happens because the framework processes CSS before Tailwind has fully compiled it, resulting in missing or incorrect styles.  This is especially relevant when using JIT compilation.

## Solution

The solution involves ensuring that Tailwind's compilation completes before the framework attempts to interpret the CSS. This usually involves correct configuration and build ordering.