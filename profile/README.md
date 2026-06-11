<p align="center">
  <img src="https://raw.githubusercontent.com/Drift-CI/drift-ci/main/assets/drift-ci-logo.png" alt="drift-ci" width="480">
</p>

<p align="center">
  <em>Catch LLM behaviour regressions in CI, before they ship.</em>
</p>

---

LLM applications drift — a reworded prompt, a model upgrade, or a bumped
dependency can silently change what your app says. **drift-ci** makes that
behaviour testable: define cases with expected outputs, score them against
your provider on every pull request, and block the merge when behaviour
drifts past a threshold — with baselines committed as code.

### Get started

​```bash
npx @drift-ci/cli init   # scaffold a suite
npx @drift-ci/cli run    # run it against your provider
​```

Or drop it into CI:

​```yaml
- uses: Drift-CI/drift-ci@v1
  with:
    provider: anthropic
    api-key: ${{ secrets.ANTHROPIC_API_KEY }}
​```

→ **[drift-ci](https://github.com/Drift-CI/drift-ci)** · [npm](https://www.npmjs.com/package/@drift-ci/cli) · [Marketplace](https://github.com/marketplace/actions/drift-ci) · [Docs](https://github.com/Drift-CI/drift-ci#readme)

