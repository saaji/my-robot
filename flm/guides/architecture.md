# Architecture

## Name abstractions and define their functions

Start with required behavior and environment. Identify responsibilities, owned state/resources, and client operations so each part can be understood through its contract. Names and directories alone establish no boundary.

Group related knowledge and decisions; hide representation choices and likely changes behind owning operations. Execution order alone does not define modules. Make data connections, control flow, coordination, and shared-resource ownership explicit.

Keep dependencies consistent with abstraction levels. Reusable lower-level parts receive needed information and operations through contracts without knowing particular higher-level callers. Shared requirements belong to their abstraction; uses to consumers ([my-requirements-flow-in-uses-flow-out](../concepts/my-requirements-flow-in-uses-flow-out.md)).

## Specify observable behavior

For each operation, specify purpose, inputs, prerequisites, results, state changes, failures, and relevant input/result/state relationships. Signatures and result-type lists cannot replace those relationships.

Separate attribute meaning and admissible values from an operation's information requirements and promises. State nested and conditional obligations at their paths. Preserve distinctions among unknown information, absence, and explicit values where the contract makes them. Data shapes need not acquire wrappers or modules.

Assess compatibility from caller obligations and guarantees. Requiring less or promising more works only while existing clients can still use the representation and behavior. Preserve additional information when the operation must carry it through.

Modules declare required dependency operations and guarantees; verify chosen providers satisfy them. Rely on upheld contracts ([my-trust-responsible-work](../concepts/my-trust-responsible-work.md)) and show how composition supports whole-system guarantees, including ordering, failure, and lifecycle.

## Keep document roles clear

Use these roles where project conditions permit:

| Role | Contract |
| --- | --- |
| Design | Subject, externally meaningful behavior, responsibilities, and relationships. |
| Specification | Detailed logical data meanings, fields/types, invariants, operations, and dependencies. |
| Blueprint | Target-stack representations, modules, storage, runtime, and integration. |

Use project vocabulary and conventions; normally place these documents in `docs/`. Keep each subject's contract in its root and chapters. Detail refers upward; high-level text remains understandable without implementation detail.

A Blueprint realizes established behavior. Resolve semantic gaps exposed by implementation in the owning Design or Specification and review affected contracts. Plans describe how to reach the target; system documents describe it with explicit status.

## Test the design against use

Check whether contracts suffice to understand, implement, test, and replace parts. Trace connections and representative success/failure paths. Investigate feasibility while keeping replaceable choices out of public promises.

Refine a considered first design from evidence ([my-design-then-refine](../concepts/my-design-then-refine.md)) and review the whole after local steps ([my-incremental-then-overhaul](../concepts/my-incremental-then-overhaul.md)). Real callers, state, and change test boundaries; document completeness alone does not.

## Original references

For fuller arguments, consult Liskov and Zilles, [Programming with Abstract Data Types](https://doi.org/10.1145/800233.807045), Liskov, [A Design Methodology for Reliable Software Systems](https://doi.org/10.1145/1479992.1480018), and Hickey, [Maybe Not](https://www.youtube.com/watch?v=YR5WdGrpoug). Distinguish their claims from an application to the current project.

links: is↑ [my-cognition-method](../topics/my-cognition-method.md)
